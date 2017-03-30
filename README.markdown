## IMCE Scala Template

The IMCE Scala Template is a Giter8 template project meant to serve as the basis for new Scala projects within the IMCE build ecosystem.

# Project Setup
1.	Use the [new template command](http://www.scala-sbt.org/0.13/docs/sbt-new-and-Templates.html) for generating a new Scala project:
```
$ sbt new JPL-IMCE/gov.nasa.jpl.imce.templates.scala.g8.git
```
2.	Follow the instructions for the particular template. We use the [reverse domain name notation convention](https://en.wikipedia.org/wiki/Reverse_domain_name_notation) for naming projects. I.e., all project names should begin with gov.nasa.jpl…
3.	Using IntelliJ or Eclipse, open the newly generated project and ensure it compiles successfully.

# GitHub Hosting

Before hosting the project on GitHub, ensure that the code has been cleared, and released for open source.
1.	Go to github.com/jpl-imce and sign in
2.	Click on “New” button, or visit https://github.com/organizations/JPL-IMCE/repositories/new
  1. Enter a repository name which matches the project name (beginning with gov.nasa.jpl…)
  2. Enter a short description of the project. Focus this description on the main functionality of the component
  3. Choose “Public” as repository type, leave the rest as default
  4. Click “Create Repository”
3.	… set remote / origin locally, do initial commit

# Bintray Publishing

There are two primary options for publishing to the [IMCE Bintray repositories](https://bintray.com/jpl-imce):
1.	Request a valid environment variable from one of the following IMCE team members: nicolas.f.rouquette@jpl.nasa.gov, sebastian.j.herzig@jpl.nasa.gov or brian.p.satorius@jpl.nasa.gov.
2.	Manually set up a Bintray account and variables. See [Two-stage publication to Bintray](https://github.com/JPL-IMCE/imce.sbt.plugin#two-stage-publication-to-bintray) for more details.
