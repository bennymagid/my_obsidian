#cicd
 Move user validation to its own spring service and globalize error throwing so that each of the controller endpoints do not need to rewrite the user validation portion
 See oauthsetup in `crud_service` - uses Spring [[Prehandle]] (can extend that class for auth)****
 Can do global user auth or per-request auth. Easiest plug-and-play solution looks to be the latter
https://www.baeldung.com/spring-security-check-user-role

 