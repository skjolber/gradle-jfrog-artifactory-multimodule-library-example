# gradle-foss-library-template
Real-world template for open-source libraries with the [Gradle] build system and JFrog Artifactory:
  
  * core libraries (my-jwt)
  * framework adaptions of core libraries
  * examples using the above
    * part of the multi-module build, but still
    * standalone, and easily copied as-is

The examples are configured as standalone applications and are not published.

Bugs, feature suggestions and help requests can be filed with the [issue-tracker].

## License
[Apache 2.0]

## Usage
Add the following properties to `~/.gradle/gradle.properties`.

```
my_artifactory_user=<email>
my_artifactory_password=<encrypted password>
my_artifactory_contextUrl=<jfrog url>
```

Build using command

> ./gradlew clean build

Publish is performed using the command 

> ./gradlew artifactoryPublish --info

# History

 - 1.0.0: Initial version

[Apache 2.0]:          			http://www.apache.org/licenses/LICENSE-2.0.html
[issue-tracker]:       			https://github.com/skjolber/gradle-foss-library-template/issues
[Gradle]:              		 	https://gradle.org/



