```
Updated com.braintreepayments.gateway:braintree-java:jar:3.37.0 to version 3.40.0
[INFO] Updated com.slack.api:slack-api-client:jar:1.28.0 to version 1.45.3
[INFO] Updated io.sentry:sentry-spring-boot-starter:jar:6.4.1 to version 8.3.0
[INFO] Updated com.pusher:pusher-http-java:jar:1.0.0 to version 1.3.4
[INFO] Updated com.amazonaws:aws-java-sdk-s3:jar:1.12.264 to version 1.12.782
[INFO] Updated org.apache.pdfbox:pdfbox:jar:2.0.27 to version 3.0.4
[INFO] Updated net.lingala.zip4j:zip4j:jar:2.11.1 to version 2.11.5
[INFO] Updated com.mailersend:java-sdk:jar:1.0.0 to version 1.0.1
[INFO] Updated org.springframework.boot:spring-boot-starter-data-jpa:jar:2.7.1 to version 3.4.3
[INFO] Updated org.springframework.boot:spring-boot-starter-oauth2-resource-server:jar:2.7.1 to version 3.4.3
[INFO] Updated org.apache.tomcat.embed:tomcat-embed-core:jar:9.0.58 to version 11.0.4
[INFO] Updated org.springframework.boot:spring-boot-starter-jdbc:jar:2.7.1 to version 3.4.3
[INFO] Updated com.vladmihalcea:hibernate-types-52:jar:2.3.5 to version 2.21.1
[INFO] Updated org.json:json:jar:20220320 to version 20250107
[INFO] Updated org.postgresql:postgresql:jar:42.3.6 to version 42.7.5
[INFO] Updated com.google.code.gson:gson:jar:2.10 to version 2.12.1
[INFO] Updated com.stripe:stripe-java:jar:20.117.0 to version 28.4.0
[INFO] Updated com.github.javadev:underscore:jar:1.77 to version 1.111
[INFO] Updated org.projectlombok:lombok:jar:1.18.24 to version 1.18.36
[INFO] Updated com.squareup.okhttp3:okhttp:jar:4.9.3 to version 5.0.0-alpha.14
[INFO] Updated com.fasterxml.jackson.core:jackson-databind:jar:2.13.3 to version 2.18.3
[INFO] Updated org.apache.commons:commons-lang3:jar:3.12.0 to version 3.17.0
[INFO] Updated commons-io:commons-io:jar:2.11.0 to version 2.18.0
[INFO] Updated com.fasterxml.jackson.datatype:jackson-datatype-jsr310:jar:2.13.3 to version 2.18.3
[INFO] Updated org.springframework:spring-beans:jar:5.3.22 to version 7.0.0-M2
```


- changed all refertences from javax to jakarta
- https://stackoverflow.com/questions/49325802/is-it-possible-to-use-hibernate-with-postgresqls-jsonb-data-type for @TypeDef Jsonb (native now in Hibernate 6+ - so we can remove open-source dependency)
- According to https://docs.sentry.io/platforms/java/guides/spring-boot/ must change sentry to jakarta version https://docs.sentry.io/platforms/java/guides/spring-boot/