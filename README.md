Spinnaker Cloud Provider Service
------------------------------------
[![Build Status](https://github.com/spinnaker/clouddriver/workflows/Branch%20Build/badge.svg)](https://github.com/spinnaker/clouddriver/actions)

This service is the main integration point for Spinnaker cloud providers like AWS, GCE, CloudFoundry, Azure etc.

### Developing with Intellij

To configure this repo as an Intellij project, run `./gradlew idea` in the root directory.

Some of the modules make use of [Lombok](https://projectlombok.org/), which will compile correctly on its own. However, for Intellij to make sense of the Lombok annotations, you'll need to install the [Lombok plugin](https://plugins.jetbrains.com/plugin/6317-lombok-plugin) as well as [check 'enable' under annotation processing](https://www.jetbrains.com/help/idea/configuring-annotation-processing.html#3).

### Debugging

To start the JVM in debug mode, set the Java system property `DEBUG=true`:
```
./gradlew -DDEBUG=true
```


The JVM will then listen for a debugger to be attached on port 7102.  The JVM will _not_ wait for
the debugger to be attached before starting Clouddriver; the relevant JVM arguments can be seen and
modified as needed in `build.gradle`.

$${\color{lightblue} Recent \space commits:}$$ 

              CommitID                   |   Author      | Commit Message          | Commit Date
----------------------------------------------------------------------------------------------------


1bc4dfade1f3ec33cd713b3e51ef1cb37bf87269 | Yugandharkumar | Create commits-preserve.yml | 2023-08-09 



62a24708669488601093b67a04ffdf7e34ccab89 | Yugandharkumar | Update README.md | 2023-08-09 