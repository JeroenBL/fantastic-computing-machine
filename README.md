# HelloID-Conn-Prov-Target-{connectorName}

> [!IMPORTANT]
> This repository contains the connector and configuration code only. The implementer is responsible to acquire the connection details such as username, password, certificate, etc. You might even need to sign a contract or agreement with the supplier before implementing this connector. Please contact the client's application manager to coordinate the connector requirements.

<p align="center">
  <img src="">
</p>

## Table of contents

- [HelloID-Conn-Prov-Target-{connectorName}](#helloid-conn-prov-target-connectorname)
  - [Table of contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Getting started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Connection settings](#connection-settings)
    - [Correlation configuration](#correlation-configuration)
    - [Field mapping](#field-mapping)
  - [Remarks](#remarks)
    - [Remark 1](#remark-1)
    - [Remark 2](#remark-2)
  - [Available lifecycle actions](#available-lifecycle-actions)
  - [API documentation](#api-documentation)
    - [Swagger](#swagger)
  - [Getting help](#getting-help)
  - [HelloID docs](#helloid-docs)

## Introduction

_HelloID-Conn-Prov-Target-{connectorName}_ is a _target_ connector. _{connectorName}_ provides a set of REST API's that allow you to programmatically interact with its data.

## Getting started

### Prerequisites

<!-- Describe the specific requirements that must be met before using this connector, such as the need for an agent, a certificate or IP whitelisting. -->

- Prerequisite 1
- Prerequisite 2

### Connection settings

The following settings are required to connect to the API.

| Setting  | Description                        | Mandatory |
| -------- | ---------------------------------- | --------- |
| UserName | The UserName to connect to the API | Yes       |
| Password | The Password to connect to the API | Yes       |
| BaseUrl  | The URL to the API                 | Yes       |

### Correlation configuration

The correlation configuration is used to specify which properties will be used to match an existing account within _{connectorName}_ to a person in _HelloID_.

| Setting                   | Value                             |
| ------------------------- | --------------------------------- |
| Enable correlation        | `True`                            |
| Person correlation field  | `PersonContext.Person.ExternalId` |
| Account correlation field | `EmployeeNumber`                  |

> [!TIP]
> _For more information on correlation, please refer to our correlation [documentation](https://docs.helloid.com/en/provisioning/target-systems/powershell-v2-target-systems/correlation.html) pages_.

### Field mapping

The field mapping can be imported by using the _fieldMapping.json_ file.

## Remarks

<!-- Provide remarks on special aspects of the code or the internal workings of the connector. -->

### Remark 1

### Remark 2

## Available lifecycle actions

The following lifecycle actions are available:

| Action                                  | Description                               |
| --------------------------------------- | ----------------------------------------- |
| create.ps1                              | PowerShell _create_ lifecycle action      |
| delete.ps1                              | PowerShell _delete_ lifecycle action      |
| disable.ps1                             | PowerShell _disable_ lifecycle action     |
| enable.ps1                              | PowerShell _enable_ lifecycle action      |
| update.ps1                              | PowerShell _update_ lifecycle action      |
| permissions/groups/grantPermission.ps1  | PowerShell _grant_ lifecycle action       |
| permissions/groups/revokePermission.ps1 | PowerShell _revoke_ lifecycle action      |
| permissions/groups/permissions.ps1      | PowerShell _permissions_ lifecycle action |
| resources/groups/resources.ps1          | PowerShell _resources_ lifecycle action   |
| configuration.json                      | Default _configuration.json_              |
| fieldMapping.json                       | Default _fieldMapping.json_               |

## API documentation

The following endpoints are used by the connector

| Endpoint | Description               |
| -------- | ------------------------- |
| /Users   | Retrieve user information |

### Swagger

<!-- If publicly available, provide the link to the swagger interface  -->

## Getting help

> [!TIP]
> _For more information on how to configure a HelloID PowerShell connector, please refer to our [documentation](https://docs.helloid.com/en/provisioning/target-systems/powershell-v2-target-systems.html) pages_.

> [!TIP]
>  _If you need help, feel free to ask questions on our [forum](https://forum.helloid.com)_.

## HelloID docs

The official HelloID documentation can be found at: https://docs.helloid.com/
