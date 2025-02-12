We get the following warning on CRUD startup

```
2025-02-10 09:56:30,428 WARN  [main] org.springframework.security.config.annotation.web.builders.WebSecurity: You are asking Spring Security to ignore Ant [pattern='/public/**']. This is not recommended -- please use permitAll via HttpSecurity#authorizeHttpRequests instead.
2025-02-10 09:56:30,428 INFO  [main] org.springframework.security.web.DefaultSecurityFilterChain: Will not secure Ant [pattern='/public/**']
2025-02-10 09:56:30,428 WARN  [main] org.springframework.security.config.annotation.web.builders.WebSecurity: You are asking Spring Security to ignore Ant [pattern='/forms/**']. This is not recommended -- please use permitAll via HttpSecurity#authorizeHttpRequests instead.
2025-02-10 09:56:30,428 INFO  [main] org.springframework.security.web.DefaultSecurityFilterChain: Will not secure Ant [pattern='/forms/**']
2025-02-10 09:56:30,428 WARN  [main] org.springframework.security.config.annotation.web.builders.WebSecurity: You are asking Spring Security to ignore Ant [pattern='/slack/**']. This is not recommended -- please use permitAll via HttpSecurity#authorizeHttpRequests instead.
2025-02-10 09:56:30,428 INFO  [main] org.springframework.security.web.DefaultSecurityFilterChain: Will not secure Ant [pattern='/slack/**']
2025-02-10 09:56:30,429 WARN  [main] org.springframework.security.config.annotation.web.builders.WebSecurity: You are asking Spring Security to ignore Ant [pattern='/close/**']. This is not recommended -- please use permitAll via HttpSecurity#authorizeHttpRequests instead.
2025-02-10 09:56:30,429 INFO  [main] org.springframework.security.web.DefaultSecurityFilterChain: Will not secure Ant [pattern='/close/**']
```