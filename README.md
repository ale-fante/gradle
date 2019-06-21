# What is Gradle

In a nutshell: Gradle is a java-based tool used to compile Android source code into artifacts.

Gradle:
- Builds artifacts (compiles Android source code into an .apk artifact)
- What are artifacts? Files (Code, Text, Graphic, audio or video)
- Manages dependencies
- What are dependencies? Ready-to-use external code and/or libraries that another company/developer wrote that provide additional functionality to a project. (SDKs can have one or multiple libraries)
- By "managing" dependencies, gradle pulls in the version of a library that is specified.
Gradle is self-updating
- New gradle versions can be obtained automatically.

Main features:
- Gradle needs a file that contains a set of detailed steps (instructions on how to create the .apk artifact (a.k.a. build).
 build.gradle is the default name for this build file and it can be found on a Jenkins build workspace. (Android build job > workspace ... build.gradle)

- Gradle reads (parses) the build.gradle file and creates a DAG (Directed Acyclic Graph) which is a fancy way of saying that it creates a graph of tasks to know what to do. It then completes each task in a one direction way: it's acyclical - the cycle doesn't repeat.
