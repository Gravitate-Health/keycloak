KEYCLOAK
=================================================
[![Build Status](https://travis-ci.org/anfederico/clairvoyant.svg?branch=master)](https://travis-ci.org/anfederico/clairvoyant)
[![License](https://img.shields.io/badge/license-Apache-blue.svg)](https://opensource.org/licenses/Apache)


Table of contents
-----------------

- [KEYCLOAK](#keycloak)
  - [Table of contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Installation](#installation)
    - [Requirements](#requirements)
    - [Deployment](#deployment)
  - [Usage](#usage)
  - [Known issues and limitations](#known-issues-and-limitations)
  - [Getting help](#getting-help)
  - [Contributing](#contributing)
  - [License](#license)
  - [Authors and history](#authors-and-history)
  - [Acknowledgments](#acknowledgments)

Introduction
------------
Keycloak is an Open Source Identity and Access Management application. This tool provides the security adding authentications to the applications with a easy mechanism. It is not an application for dealing with storing users or their authentications. Users authenticate with Keycloak rather than individual applications. Once logged-in to Keycloak, users don't have to login again to access a different application.

Installation
------------
### Requirements
To deploy keycloak is necessary to have installed previously JAVA 11 JRE. 

### Deployment
First of all, we need to install our server in the [Keycloak Download](https://www.keycloak.org/documentation) to set it up locally. There are different options to do it, but in this deployment it will be choose the _.zip_ format. 

When the _.zip_ is downloaded, it is necessary to extract the content. We open the folder extracted and open a terminal with the following command:

```bash
> cd path/keycloak-17.0.1/keycloak-17.0.1/bin
```
Once this is done, we are going to start the server, to access to the keycloak interface. 

```bash
> .\kc.bat start-dev
```
This command will respond with the localhost URL where is runnig our server, as follows http://127.0.0.x:8080. If we access with a browser, the keycloak interface will welcome us. In the first access is necessary to create an account by adding a username/email and a password. Once authenticated, the configuration interface of keycloak appears at the Master Realm.

![Keycloak Welcome Interface](./img/welcome.png)

A **Realm** is an object that manage a set of of users, credentials, roles, and groups. A user in Keycloak belongs to only one realm and the user who logs in to Keycloak will log into that user's realm. The Master Realm contains the administrator account 

Usage
-----
Now, 

Known issues and limitations
----------------------------

Getting help
------------
In case you find a problem or you need extra help, please use the issues tab to report the issue.

Contributing
------------
To contribute, fork this repository and send a pull request with the changes squashed.

License
------------
```
This project is distributed under the terms of the [Apache License, Version 2.0 (AL2)](https://www.apache.org/licenses/LICENSE-2.0).  The license applies to this file and other files in the [GitHub repository](https://github.com/Gravitate-Health/fhir-connector) hosting this file.

Copyright 2022 Universidad Politécnica de Madrid

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

Authors and history
---------------------------
- Isabel Varona ([@isabelvato](https://github.com/isabelvato))
- 
Acknowledgments
---------------------------
- [Keycloak Documentation](https://www.keycloak.org/documentation)
  