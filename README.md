# org.lthn.sdp.api

## Requirements

Building the API client library requires [Maven](https://maven.apache.org/) to be installed.

## Installation

To install the API client library to your local Maven repository, simply execute:

```shell
mvn install
```

To deploy it to a remote Maven repository instead, configure the settings of the repository and execute:

```shell
mvn deploy
```

Refer to the [official documentation](https://maven.apache.org/plugins/maven-deploy-plugin/usage.html) for more information.

### Maven users

Add this dependency to your project's POM:

```xml
<dependency>
    <groupId>lethean</groupId>
    <artifactId>org.lthn.sdp.api</artifactId>
    <version>1.0.0</version>
    <scope>compile</scope>
</dependency>
```

### Gradle users

Add this dependency to your project's build file:

```groovy
compile "lethean:org.lthn.sdp.api:1.0.0"
```

### Others

At first generate the JAR by executing:

    mvn package

Then manually install the following JARs:

- target/org.lthn.sdp.api-1.0.0.jar
- target/lib/*.jar

## Getting Started

Please follow the [installation](#installation) instruction and execute the following Java code:

```java

import org.lthn.sdp.api.VpnApi;

public class VpnApiExample {

    public static void main(String[] args) {
        VpnApi apiInstance = new VpnApi();
        String dataDir = null; // String | Returns the binary version
        Boolean version = null; // Boolean | Returns the binary version
        try {
            apiInstance.startLetheand(dataDir, version);
        } catch (ApiException e) {
            System.err.println("Exception when calling VpnApi#startLetheand");
            e.printStackTrace();
        }
    }
}

```

## Documentation for API Endpoints

All URIs are relative to *http://localhost*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*VpnApi* | [**startLetheand**](docs/VpnApi.md#startLetheand) | **GET** /letheand/start | 


## Documentation for Models



## Documentation for Authorization

All endpoints do not require authorization.
Authentication schemes defined for the API:

## Recommendation

It's recommended to create an instance of `ApiClient` per thread in a multithreaded environment to avoid any potential issues.

## Author

contact@lethean.io

