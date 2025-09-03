#cicd
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

There is a branch to handle the above `crud-service/benny/security-tests`
https://gitlab.com/coverdash/crud_service/-/merge_requests/310

Our prod runners use `.properties` files which must be uploaded -in addition to the `.jar` - to our remote servers. 
This means 
1. we are committing our entire properties file (with passwords and keys for anyone to find!)
2. These properties files are on our remote similarly not secured
3. We can have a drift between the repo's version of the properties file and the remote version
https://chatgpt.com/share/67b74c97-5aa0-8006-a616-84bf76e8fa8b