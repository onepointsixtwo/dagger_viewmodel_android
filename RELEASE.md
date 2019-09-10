# Release

## Pre-Requisites

The pre-requisites for releasing this are as follows:

1. The GPG key must be set (this is backed up).

2. There must be a global or local gradle configuration setup with the values ossrhUser, ossrhPassword for your sonatype username and password.


## Upload

Simply run the command `./gradlew uploadArchives` to upload the aar to maven central (nexus). Use
`./gradlew closeAndPromoteRepository` to actually release it.

You can login to Sonatype and look at 'Staging Repositories' to see that it has uploaded between
these steps.
