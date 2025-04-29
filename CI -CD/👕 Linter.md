My favorite combination is

- [google-java-format](https://github.com/google/google-java-format) for auto-formatting (prevent bikeshedding about indentation and the like)
	- Installed in Intellij
	- Enabled manually in settings
	- Updated JRE Config
	- Reformat on save
	- Added dependency to Maven
```
<dependency>  
    <groupId>com.google.googlejavaformat</groupId>  
    <artifactId>google-java-format</artifactId>  
    <version>1.25.2</version>  
</dependency>
```
	
	- Added to Maven to check on commit
Run this once - look at [this article](https://aru-sha4.medium.com/java-check-style-and-formatting-using-maven-a1a1b4e6e10a)
check here too for the [xml](https://github.com/checkstyle/checkstyle/blob/master/src/main/resources/google_checks.xml)


```
<plugin>  
    <groupId>com.theoryinpractise</groupId>  
    <artifactId>googleformatter-maven-plugin</artifactId>  
    <version>1.7.3</version>  
    <executions>  
        <execution>  
            <id>reformat-sources</id>  
            <configuration>  
                <includeStale>false</includeStale>  
                <style>GOOGLE</style>  
                <!--                            <formatMain>true</formatMain>-->  
                <!--                            <formatTest>true</formatTest>-->                <filterModified>false</filterModified>  
                <skip>false</skip>  
                <fixImports>false</fixImports>  
                <maxLineLength>100</maxLineLength>  
            </configuration>  
            <goals>  
                <goal>format</goal>  
            </goals>  
            <phase>process-sources</phase>  
        </execution>  
    </executions>  
</plugin>
```
- [checkstyle](https://maven.apache.org/plugins/maven-checkstyle-plugin/index.html) with google-java-format rules (this is also where we could specify unused imports)
- [errorprone](https://errorprone.info/) (prevent common, careless mistakes)
- [NullAway](https://github.com/uber/NullAway) (prevent NullPointerExceptions)
- [infer](https://fbinfer.com/) (optionally) to be really safe :)

In my opinion, linters should be executable via the command-line. Hence i don't like SonarQube and sonalint. For SonarQube you need a server running somewhere and sent the reports over the wire. It's also really slow and can double or even triple the build time. Sonalint is only pluggable into a IDE like Intellij or VS Code but not runnable from the CLI. Both Sona-tools remind me too much of big fat enterprise tooling. Further my favorite editor Emacs is not supported :)

Recently i created a template java-quarkus project as a showcase which integrates all the above linters, see [https://github.com/gerlacdt/quarkus-playground](https://github.com/gerlacdt/quarkus-playground)