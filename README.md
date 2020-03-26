# GraphQL Spring Webclient

Reactive GraphQL client for consuming GraphQL APIs from a Spring Boot application.
Provides OAuth2 authorization through configuration.

## Getting started

Add the starter to your project.

When using Maven:
```xml
<dependency>
  <groupId>com.graphql-java-kickstart</groupId>
  <artifactId>graphql-webclient-spring-boot-starter</artifactId>
  <version>1.0.0-SNAPSHOT</version>
</dependency>
```

When using gradle:
```groovy
implementation "com.graphql-java-kickstart:graphql-webclient-spring-boot-starter:1.0.0-SNAPSHOT"
```

Configure at least the URL of the GraphQL API to consume:
```yaml
graphql:
  client:
    url: https://graphql.github.com/graphql
```

## Configuration

The following tables list the configurable properties of the GraphQL Spring Webclient and their default values.
These properties are configured with the prefix `graphql.client`, e.g. the property listed in the table as `url` 
should be defined as `graphql.client.url` in your Spring Boot configuration files.

| Property | Description |
|----------|-------------|
| url | Full URL of the GraphQL API to connect to, e.g. https://graphql.github.com/graphql |
| oauth2.client-id | OAuth2 client id |
| oauth2.client-secret | OAuth2 client secret |
| oauth2.token-uri | Token URI of the identity provider |
| oauth2.authorization-grant-type | By default the grant type `client_credentials` is used |
 

