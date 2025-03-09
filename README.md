# TalkOps SDK: NodeJS

This software development kit is made to create [TalkOps](https://link.talkops.app/talkops) Extension.

## Documentation

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

#### Table of Contents

*   [Alarm](#alarm)
*   [Extension](#extension)
    *   [Parameters](#parameters)
    *   [setInstructions](#setinstructions)
        *   [Parameters](#parameters-1)
    *   [setFunctionSchemas](#setfunctionschemas)
        *   [Parameters](#parameters-2)
    *   [setFunctions](#setfunctions)
        *   [Parameters](#parameters-3)
*   [Message](#message)
    *   [setText](#settext)
        *   [Parameters](#parameters-4)
    *   [setFrom](#setfrom)
        *   [Parameters](#parameters-5)
    *   [addTo](#addto)
        *   [Parameters](#parameters-6)
*   [Module](#module)
    *   [Parameters](#parameters-7)
    *   [setVersion](#setversion)
        *   [Parameters](#parameters-8)
    *   [setDescription](#setdescription)
        *   [Parameters](#parameters-9)
    *   [setInstallationGuide](#setinstallationguide)
        *   [Parameters](#parameters-10)
    *   [setEnvironmentVariables](#setenvironmentvariables)
        *   [Parameters](#parameters-11)
    *   [setDockerRepository](#setdockerrepository)
        *   [Parameters](#parameters-12)
    *   [setDockerVolumeData](#setdockervolumedata)
        *   [Parameters](#parameters-13)
*   [Levels](#levels)
*   [Notification](#notification)
    *   [setLevel](#setlevel)
        *   [Parameters](#parameters-14)
*   [Readme](#readme)
    *   [Parameters](#parameters-15)
*   [Service](#service)
    *   [Parameters](#parameters-16)
    *   [send](#send)
        *   [Parameters](#parameters-17)

### Alarm

**Extends Message**

Represents an alarm.

### Extension

**Extends Module**

Represents an extension.

#### Parameters

*   `name` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The name of the extension.

#### setInstructions

##### Parameters

*   `instructions` **([String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String) | [Array](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array)<[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)> | [Function](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Statements/function) | AsyncFunction)** The instructions of the extension for the AI agent.

#### setFunctionSchemas

##### Parameters

*   `functionSchemas` **([Array](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array)<[Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)> | [Function](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Statements/function) | AsyncFunction)** The function schemas of the extension for the AI agent.

#### setFunctions

##### Parameters

*   `functions` **[Array](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array)<([Function](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Statements/function) | AsyncFunction)>** The named functions of the extension.

### Message

Represents a message.

#### setText

##### Parameters

*   `text` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The text of the message.

Returns **[Message](#message)** The updated message instance.

#### setFrom

##### Parameters

*   `emitter` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The emitter of the message.

Returns **[Message](#message)** The updated message instance.

#### addTo

##### Parameters

*   `clientId` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The client target unique identifier of the message.

Returns **[Message](#message)** The updated message instance.

### Module

Represents a module.

#### Parameters

*   `name` &#x20;
*   `type` &#x20;

#### setVersion

##### Parameters

*   `version` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The version of the module.

#### setDescription

##### Parameters

*   `description` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The description of the module.

#### setInstallationGuide

##### Parameters

*   `installationGuide` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The installation guide of the module.

#### setEnvironmentVariables

##### Parameters

*   `environmentVariables` **[Array](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array)<[Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)>** The environment variables of the extension.

#### setDockerRepository

##### Parameters

*   `dockerRepository` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The docker repository of the extension.

#### setDockerVolumeData

##### Parameters

*   `dockerVolumeData` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The docker volume data of the extension.

### Levels

Represents levels for a notification.

Type: [string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)

### Notification

**Extends Message**

Represents a notification.

#### setLevel

##### Parameters

*   `level` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The level of the notification (low, normal, high, critical).

Returns **[Notification](#notification)** The updated notification instance.

### Readme

Represents a readme.

#### Parameters

*   `templateUrl` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The template URL.
*   `path` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The path of the readme file.
*   `module` **[Module](#module)** The module (e.g. an extension).

### Service

Represents a service.

#### Parameters

*   `agentUrls` **[Array](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array)<[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)>** The agent URLs.
*   `modules` **([Module](#module) | [Array](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array)<[Module](#module)>)** The modules (e.g. an extension).

#### send

##### Parameters

*   `messages` **([Message](#message) | [Array](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array)<[Message](#message)>)** The messages.
