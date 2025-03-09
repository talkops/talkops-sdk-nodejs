# TalkOps SDK: NodeJS

## Documentation

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

#### Table of Contents

*   [Extension](#extension)
    *   [Parameters](#parameters)
    *   [setInstructions](#setinstructions)
        *   [Parameters](#parameters-1)
    *   [setFunctionSchemas](#setfunctionschemas)
        *   [Parameters](#parameters-2)
    *   [setFunctions](#setfunctions)
        *   [Parameters](#parameters-3)
*   [Module](#module)
    *   [Parameters](#parameters-4)
    *   [setVersion](#setversion)
        *   [Parameters](#parameters-5)
    *   [setDescription](#setdescription)
        *   [Parameters](#parameters-6)
    *   [setInstallationGuide](#setinstallationguide)
        *   [Parameters](#parameters-7)
    *   [setEnvironmentVariables](#setenvironmentvariables)
        *   [Parameters](#parameters-8)
    *   [setDockerRepository](#setdockerrepository)
        *   [Parameters](#parameters-9)
    *   [setDockerVolumeData](#setdockervolumedata)
        *   [Parameters](#parameters-10)
*   [Readme](#readme)
    *   [Parameters](#parameters-11)
*   [Service](#service)
    *   [Parameters](#parameters-12)

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
*   `modules` **([Module](#module) | [String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)<[Module](#module)>)** The modules (e.g. an extension).
