# TalkOps SDK: NodeJS

This software development kit is made to create [TalkOps](https://link.talkops.app/talkops) Extension.

## Documentation

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

#### Table of Contents

*   [Alarm](#alarm)
*   [Event](#event)
    *   [setFrom](#setfrom)
        *   [Parameters](#parameters)
    *   [addTo](#addto)
        *   [Parameters](#parameters-1)
*   [Extension](#extension)
    *   [Parameters](#parameters-2)
    *   [setInstructions](#setinstructions)
        *   [Parameters](#parameters-3)
    *   [setFunctionSchemas](#setfunctionschemas)
        *   [Parameters](#parameters-4)
    *   [setFunctions](#setfunctions)
        *   [Parameters](#parameters-5)
*   [Message](#message)
    *   [setText](#settext)
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
    *   [enableDockerVolumeData](#enabledockervolumedata)
    *   [disableDockerVolumeData](#disabledockervolumedata)
*   [Notification](#notification)
    *   [setLevel](#setlevel)
        *   [Parameters](#parameters-13)
*   [Readme](#readme)
    *   [Parameters](#parameters-14)
*   [Service](#service)
    *   [Parameters](#parameters-15)
    *   [send](#send)
        *   [Parameters](#parameters-16)

### Alarm

**Extends Event**

Represents an alarm.

### Event

Represents an event.

#### setFrom

##### Parameters

*   `emitter` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The emitter of the event.

Returns **[Event](#event)** The updated event instance.

#### addTo

##### Parameters

*   `clientId` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The client target unique identifier of the event.

Returns **[Event](#event)** The updated event instance.

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

**Extends Event**

Represents a message.

#### setText

##### Parameters

*   `text` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The text of the message.

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

#### enableDockerVolumeData

Enable the docker volume data.

#### disableDockerVolumeData

Disable the docker volume data.

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

Send one or more events.

##### Parameters

*   `events` **([Event](#event) | [Array](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array)<[Event](#event)>)** The events.
