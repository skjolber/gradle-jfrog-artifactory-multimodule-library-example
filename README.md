# gradle-jfrog-artifactory-multimodule-library-example
Real-world template for open-source libraries with the [Gradle] build system and JFrog Artifactory using the [Gradle Artifactory Plugin]:
  
  * core libraries (my-jwt)
  * framework adaptions of core libraries
  * examples using the above
    * part of the multi-module build, but still
    * standalone, and easily copied as-is

The examples are not published. 

Bugs, feature suggestions and help requests can be filed with the [issue-tracker].

## License
[Apache 2.0]

## Usage
Add the following properties to your global gradle properties at `~/.gradle/gradle.properties`:

```
my_artifactory_user=<email>
my_artifactory_password=<encrypted password>
my_artifactory_contextUrl=<jfrog url>
```

Build using command

> ./gradlew clean build --info

Publish is performed using the command 

> ./gradlew artifactoryPublish --info

# See also

  * Corresponding example using Maven Central: [gradle-sonatype-oss-multimodule-library-example]

# History

 - 1.0.1: Bumped dependencies, renamed project.
 - 1.0.0: Initial version

[Apache 2.0]:          			http://www.apache.org/licenses/LICENSE-2.0.html
[issue-tracker]:       			https://github.com/skjolber/gradle-foss-library-template/issues
[Gradle]:              		 	https://gradle.org/
[Gradle Artifactory Plugin]:                    https://www.jfrog.com/confluence/display/JFROG/Gradle+Artifactory+Plugin
[gradle-sonatype-oss-multimodule-library-example]: https://github.com/skjolber/gradle-sonatype-oss-multimodule-library-example


