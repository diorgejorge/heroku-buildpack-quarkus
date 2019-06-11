# heroku-buildpack-quarkus

This is a [Heroku Buildpack](https://devcenter.heroku.com/articles/buildpacks) for running [Quarkus](https://quarkus.io).

## Usage

Put your JAR file(s) in `target/` and deploy.

## Using with the Java buildpack

You can use the standard Heroku Java buildpack to package your JAR file, and then run it using java -jar :

```sh-session
$ heroku buildpacks:clear
$ heroku buildpacks:add heroku/java
$ heroku buildpacks:add https://github.com/micha-van-santvoort/heroku-buildpack-quarkus
```
