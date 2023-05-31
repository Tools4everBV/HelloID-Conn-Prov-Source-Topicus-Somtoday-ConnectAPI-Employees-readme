# HelloID-Conn-Prov-Source-Topicus-Somtoday-ConnectAPI-Employees-readme

| :warning: Warning - **You need to sign a contract with the supplier before implementing this connector**|
|:---------------------------|
| This repository contains the connector and configuration code only. The implementer is responsible to acquire the connection details such as username, password, certificate, etc. Please contact the client's application manager to coordinate the connector requirements.       |

| :information_source: Contact |
|:---------------------------|
| Please contact your local Tools4ever sales representative for further information and details about the implementation of this connector  |

<br />
<p align="center">
  <img src="assets/logo.png">
</p>

## Table of contents

- [Introduction](#Introduction)
- [Getting started](#Getting-started)
  + [Connection settings](#Connection-settings)
  + [Prerequisites](#Prerequisites)
  + [Remarks](#Remarks)
- [Setup the connector](@Setup-The-Connector)
- [Getting help](#Getting-help)
- [HelloID Docs](#HelloID-docs)

## Introduction

_HelloID-Conn-Prov-Source-Topicus-Somtoday-Employee_ is a _source_ connector. Topicus-Somtoday-Employee provides a set of REST API's that allow you to programmatically interact with it's data. The connector retrieves Employees from SOMToday. This connector cannot be used as a 'Core' HR system. Because the API does not return employment data or start and end date for each employee. The only dates you can find are the schoolyears. You can use this connector in addition to your current HR system.

## Getting started

### Connection settings

The following settings are required to connect to the API.

| Setting      | Description                        | Mandatory   |
| ------------ | -----------                        | ----------- |
| ClientID     | The ClientID to connect to the API | Yes         |
| ClientSecret | The Password to connect to the API | Yes         |
| BaseUrl      | The URL to the API                 | Yes         |
| Instelling   | The Name of the organization       | Yes         |
| schoolYear   | Specify the period to receive employees (HUIDIG and VOLGEND)     | No         | (Script variable)

### Prerequisites
 - As implementer, you need your own set of credentials before you can implement this connector. Therefore you need to sign a contract with the supplier.
 - Custom HelloID Contract field named "Leerjaar"  > [ManageCustomFields](https://docs.helloid.com/hc/en-us/articles/360012913319-Create-and-manage-custom-fields)

### Remarks
 - The API does not contain employment information, so only the persons and their subject choices are retrieved from SOMToday. The subject choices are added as HelloID contracts and enriched with extra subject information.


## Setup the connector

## Getting help

> _For more information on how to configure a HelloID PowerShell connector, please refer to our [documentation](https://docs.helloid.com/hc/en-us/articles/360012557600-Configure-a-custom-PowerShell-source-system) pages_

> _If you need help, feel free to ask questions on our [forum](https://forum.helloid.com)_

## HelloID docs

The official HelloID documentation can be found at: https://docs.helloid.com/
