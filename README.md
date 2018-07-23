# Heroku Buildpack Wildfly Standalone

## Using with Gradle buildpack

You can use the standard Heroku Gradle buildpack to compile your WAR file, 
and then have wildfly run it:

```bash
$ heroku buildpacks:clear
$ heroku buildpacks:add heroku/gradle
$ heroku buildpacks:add https://github.com/WeTrustPlatform/heroku-buildpack-wildfly-standalone.git
```