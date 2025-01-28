See [[🚀 Release Process SoTA]]
There ought to be some GitLab Action that can automate the process

When running the `run` shell script for a given service, we have to switch users from `ubuntu` to `root` using `sudo su`. This effectively lets us run all subsequent commands a `root` which is dangerous (i.e. any file can be irrevocably deleted). We do this because if you try to run / restart a service now with a non-`root` user like `ubuntu`, you'll get an error when trying to create / write to the `logs` file (e.g. `logs/crud_service_logs` - a path specified in `logback-spring.xml` - because the logs file is in the `root` owner and group).

To fix: change the log file for each service (in every environment) to be owned by and in the group of `ubuntu` - then we won't have to run commands as `root` anymore
`chown -R ubuntu:ubuntu logs/crud_service.log` 
For now, instead we opted only to `sudo` for the restart command itself - can write some shortcuts in `.bashrc`, but I had an issue with this being run from the root directory

I get the following when I run the bashrc from root folder
```org.springframework.context.ApplicationContextException: Unable to start web server; nested exception is org.springframework.boot.web.server.WebServerException: Unable to start embedded Tomcat
        at org.springframework.boot.web.servlet.context.ServletWebServerApplicationContext.onRefresh(ServletWebServerApplicationContext.java:165) ~[spring-boot-2.7.3.jar!/:2.7.3]
        at org.springframework.context.support.AbstractApplicationContext.refresh(AbstractApplicationContext.java:577) ~[spring-context-5.3.22.jar!/:5.3.22]
        at org.springframework.boot.web.servlet.context.ServletWebServerApplicationContext.refresh(ServletWebServerApplicationContext.java:147) ~[spring-boot-2.7.3.jar!/:2.7.3]
        at org.springframework.boot.SpringApplication.refresh(SpringApplication.java:734) ~[spring-boot-2.7.3.jar!/:2.7.3]
        at org.springframework.boot.SpringApplication.refreshContext(SpringApplication.java:408) ~[spring-boot-2.7.3.jar!/:2.7.3]
        at org.springframework.boot.SpringApplication.run(SpringApplication.java:308) ~[spring-boot-2.7.3.jar!/:2.7.3]
        at org.springframework.boot.SpringApplication.run(SpringApplication.java:1306) ~[spring-boot-2.7.3.jar!/:2.7.3]
        at org.springframework.boot.SpringApplication.run(SpringApplication.java:1295) ~[spring-boot-2.7.3.jar!/:2.7.3]
        at com.coverdash.lead_assignment_service.LeadAssignmentServiceApplication.main(LeadAssignmentServiceApplication.java:57) ~[classes!/:1.11]
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[na:na]
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[na:na]
        at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[na:na]
        at java.base/java.lang.reflect.Method.invoke(Method.java:566) ~[na:na]
        at org.springframework.boot.loader.MainMethodRunner.run(MainMethodRunner.java:49) ~[lead_assignment_service.jar:1.11]
        at org.springframework.boot.loader.Launcher.launch(Launcher.java:108) ~[lead_assignment_service.jar:1.11]
        at org.springframework.boot.loader.Launcher.launch(Launcher.java:58) ~[lead_assignment_service.jar:1.11]
        at org.springframework.boot.loader.JarLauncher.main(JarLauncher.java:65) ~[lead_assignment_service.jar:1.11]
```