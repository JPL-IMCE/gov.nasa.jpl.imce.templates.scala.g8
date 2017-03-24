## IMCE Scala Template

The IMCE Scala Template is a Giter8 template project meant to serve as the basis for new Scala projects within the IMCE build ecosystem.

# Project Setup
1.	Use the [Giter8 command ](http://www.foundweekends.org/giter8/setup.html) for generating a new Scala project:
  ```$ g8 JPL-IMCE/gov.nasa.jpl.imce.templates.scala.g8.git```
2.	Follow the instructions for the particular template. We use the [reverse domain name notation convention](https://en.wikipedia.org/wiki/Reverse_domain_name_notation) for naming projects. I.e., all project names should begin with gov.nasa.jpl…
3.	Using IntelliJ or Eclipse, open the newly generated project and ensure it compiles successfully.

# GitHub Hosting

Before hosting the project on GitHub, ensure that the code has been cleared, and released for open source.
1.	Go to github.com/jpl-imce and sign in
2.	Click on “New” button, or visit https://github.com/organizations/JPL-IMCE/repositories/new
  a.	Enter a repository name which matches the project name (beginning with gov.nasa.jpl…)
  b.	Enter a short description of the project. Focus this description on the main functionality of the component
  c.	Choose “Public” as repository type, leave the rest as default
  d.	Click “Create Repository”
3.	… set remote / origin locally, do initial commit
