# Reddio Java SDK

For downloading the latest version of the SDK, please visit the [Releases](https://github.com/reddio-com/reddio-java-sdk/releases).

## Usage

Download the latest version of java SDK from [Releases Page](https://github.com/reddio-com/reddio-java-sdk/releases)

Execute the following command to install the SDK to local maven repository.

```bash
## replace with the version you downloaded, keep the SNAPSHOT suffix
export VERSION="0.0.2-SNAPSHOT" 
unzip reddio-java-sdk.zip
mvn install:install-file -Dfile=./reddio-api/target/reddio-api-${VERSION}.jar -Dsource=./reddio-api/target/reddio-api-${VERSION}-sources.jar -Djavadoc=./reddio-api/target/reddio-api-${VERSION}-javadoc.jar -DgroupId=com.reddio -DartifactId=reddio-api -Dversion=${VERSION} -Dpackaging=jar
mvn install:install-file -Dfile=./reddio-crypto/target/reddio-crypto-${VERSION}.jar -Dsource=./reddio-crypto/target/reddio-crypto-${VERSION}-sources.jar -Djavadoc=./reddio-crypto/target/reddio-crypto-${VERSION}-javadoc.jar -DgroupId=com.reddio -DartifactId=reddio-crypto -Dversion=${VERSION} -Dpackaging=jar
```
