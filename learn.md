# Openshift Deploy Tools

![Almatoolbox Logo](http://logoshabm.tmdb.de/240/015095847.JPG "Almatoolbox Logo")

## Build starter
![Build-starter-screen](/screenshots/start-build.jpg?raw=true "Build starter")
### Fieldset explanation
#### Token
Relative path of file containing the security token of your Openshift project, stored in your repository.
#### Buildconfig
Name of build configuration to start
#### Namespace
Openshift project to build against
#### Openshift Connection
##### Client executable
Path to oc client
##### Target server
Openshift hostname and port
##### Username & Password
Openshift credentials
*one of username&password or Client Certificate must be specified*
##### Client Certificate
Path to client certificate
*one of username&password or Client Certificate must be specified*
##### Skip TLS Verify
Tells oc to insecurely skip TLS verification.

#### Further reading
[The Openshift Developer's guide - Starting a Build](https://docs.openshift.com/enterprise/3.1/dev_guide/builds.html#starting-a-build) 

## Image Tagger
![Image-tagger-screen](/screenshots/tag.jpg?raw=true "Tagger")
### Fieldset explanation
#### Source image
Existing tag or image from an image stream, or a Docker image pull spec.
#### Target
Target image stream
#### Openshift Connection
##### Client executable
Path to oc client
##### Target server
Openshift hostname and port
##### Username & Password
Openshift credentials
*one of username&password or Client Certificate must be specified*
##### Client Certificate
Path to client certificate
*one of username&password or Client Certificate must be specified*
##### Skip TLS Verify
Tells oc to insecurely skip TLS verification.

#### Further reading
[The Openshift Developer's guide - Tag CLI Reference](https://docs.openshift.com/enterprise/3.1/cli_reference/basic_cli_operations.html#tag) 

## Image promoter
![Promoter-screen](/screenshots/promote.jpg?raw=true "Promoter")
### Fieldset explanation
#### Openshift Docker Registry
Openshift dev Docker Registry to pull from
#### Source Tag
Tagged image ready for production
#### Target Tag
Destination tag (e.g. source image will be tagged with this value in target - production - environment)
#### Docker machine
Docker client host used for pulling and pushing
#### Username
SSH user
#### Password
SSH password

