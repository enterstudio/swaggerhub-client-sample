### Swaggerhub Client Sample

[![Build Status](https://travis-ci.org/fehguy/swaggerhub-client-sample.svg)](https://travis-ci.org/fehguy/swaggerhub-client-sample)

This is an example for introducing swaggerhub into the workflow of generating an API client.
It is based on a public API definition:

https://swaggerhub.com/api/fehguy/swaggerhub-sample/1.0.0

The project has a single profile to pull down the swagger definition from the SwaggerHub API, then
use it for codegen processes.  You can invoke this by using the `regen` profile:

```
mvn package -Pregen
```

This causes the `src/gen/java` folder to be updated against the latest data from the swaggerhub definition.