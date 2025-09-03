#cicd
[Here](https://medium.com/@AlexanderObregon/enhancing-logging-with-log-and-slf4j-in-spring-boot-applications-f7e70c6e4cc7) is an overview on logging with
Lombok
Spring
SL4J
1. Do we return a bad response like a 403?
2. Is Sentry notified?
3. Do we return a 200 and just log the error
4. log.info vs log.error
5. log messages to users are confusing too

According to Perry, we generally prefer sending 200 response always but with an `Error` key instead of a `400` (although we send that all the time)because a `400` means that the page reloads (can be destructive if filling out a form for example)

For inputs to Controllers, can we define a method (maybe in `CoverdashRestController`) that helps validate a set of inputs? If we use a shared component, can we make this happen automatically?