# IMCE Project Template

The IMCE Project Template is a Giter8 template project serving as the basis for new Scala projects within the IMCE build ecosystem. 

Meant for developers familiar with or new to the IMCE platform, this repository contains reference guides and general purpose build and publish scripts for integration with IMCE accounts on Travis CI, Bintray and Github.

## Prerequisites
#### Git
Download and install Git using the installers from [here](https://git-scm.com/downloads).
#### Oracle JDK
Oracle JDK, the Java Development Kit, version 1.8. Check you have the right version by typing in the console:
```
$ java -version
```
If necessary, download the .tar.gz archive from the [Oracle website](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) and follow the installation steps for your operating system.
#### sbt

[Follow the instructions for your platform](http://www.scala-sbt.org/release/docs/Setup.html) to get sbt running.

IMCE requires sbt version 0.13.x. If in doubt, you can check your currently installed sbt by running:
```
$ sbt about
```
#### IDE
[Intellij IDEA](https://www.jetbrains.com/idea/download/), [Scala IDE for Eclipse](http://scala-ide.org/), or another IDE of your choice.

## Documentation
* [Github Hosting](src/main/g8/github_hosting.md) - Setup documentation including setup, configuration, and reference material
* [Bintray Publishing](src/main/g8/bintray_publishing.md) - Developer documentation including setup and reference material
* [Travis CI Integration](src/main/g8/travis_ci_integration.md) - Integration instructions for linking to a Travis CI account.

## Project Setup
1.	Use the [new template command](http://www.scala-sbt.org/0.13/docs/sbt-new-and-Templates.html) for generating a new Scala project:
```
$ sbt new JPL-IMCE/gov.nasa.jpl.imce.templates.scala.g8.git
```
2.	Follow the instructions for the particular template. We use the [reverse domain name notation convention](https://en.wikipedia.org/wiki/Reverse_domain_name_notation) for naming projects. I.e., all project names should begin with gov.nasa.jpl…
3.	Using IntelliJ or Eclipse, open the newly generated project and ensure it compiles successfully.

