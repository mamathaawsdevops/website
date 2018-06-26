---
reviewers:
- chenopis
layout: docsportal
css: /css/style_user_journeys.css
js: https://use.fontawesome.com/4bcc658a89.js, https://cdnjs.cloudflare.com/ajax/libs/prefixfree/1.0.7/prefixfree.min.js, https://cloud.google.com/js/embed.min.js
title: Foundational
track: "USERS › APPLICATION DEVELOPER › FOUNDATIONAL"
content_template: templates/user-journey-content
---

{{% capture overview %}}


## Basic Concepts

### Container

_Containers_ are objects that contain everything required (such as code, system tools, system libraries, settings) to run an application. A container is an active instantiation of an image.

Containers sit on a physical or virtual host machine and run on the host’s operating system. This makes containers lightweight and portable: only megabytes in size. Containers help ensure that applications deploy quickly and reliably unlike virtual machines which are bulky and take a longer time to reboot.

Example:

### Image

_An Image_ is a binary package that encapsulates all of the files necessary to run an application inside of an OS container.{Do I need to site this?}  
For better understanding, you can think of an image as a class in a programming language and a container as an instance of that class.


### Container Engine

_Container Engine_ is a system for automating deployment, scaling, and management of containerized applications. Container engine provisions the compute resources required by the application after a user specifies them. A container engine instantiates an image into a container.

### Control Loop/ Reconciliation Loop

_Control Loop_ is a non-terminating loop that regulates the state of the system through the apiserver and makes changes attempting to move the current state towards the desired state.

Example: If there are currently 2 pods (current state) running in a node, however you want 3 additional pods(desired state) in a node, control loop ensures to spin up 3 additional pods