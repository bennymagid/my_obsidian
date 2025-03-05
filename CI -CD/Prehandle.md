Consider using prehandle for logging when a mehod is called at all
```
import jakarta.servlet.http.HttpServletRequest;
import jakarta.servlet.http.HttpServletResponse;
import org.slf4j.Logger;
import org.slf4j.LoggerFactory;
import org.springframework.web.servlet.HandlerInterceptor;
import org.springframework.web.method.HandlerMethod;

public class CoverdashLoggingInterceptor implements HandlerInterceptor {
    private static final Logger logger = LoggerFactory.getLogger(CoverdashLoggingInterceptor.class);

    @Override
    public boolean preHandle(HttpServletRequest request, HttpServletResponse response, Object handler) {
        if (handler instanceof HandlerMethod handlerMethod) {
            Class<?> controllerClass = handlerMethod.getBeanType();
            if (CoverdashRestController.class.isAssignableFrom(controllerClass)) {
                logger.info("Called: {} with args: {}", handlerMethod.getMethod().getName(), request.getParameterMap());
            }
        }
        return true; // Continue request processing
    }
}
```