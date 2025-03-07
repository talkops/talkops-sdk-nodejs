<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

*   [Extension][1]
    *   [Parameters][2]
    *   [setInstructions][3]
        *   [Parameters][4]
    *   [setFunctionSchemas][5]
        *   [Parameters][6]
    *   [setFunctions][7]
        *   [Parameters][8]
*   [Module][9]
    *   [Parameters][10]
    *   [setVersion][11]
        *   [Parameters][12]
    *   [setDescription][13]
        *   [Parameters][14]
    *   [setInstallationGuide][15]
        *   [Parameters][16]
    *   [setEnvironmentVariables][17]
        *   [Parameters][18]
    *   [setDockerRepository][19]
        *   [Parameters][20]
    *   [setDockerVolumeData][21]
        *   [Parameters][22]
*   [Readme][23]
    *   [Parameters][24]
*   [Service][25]
    *   [Parameters][26]

## Extension

**Extends Module**

Represents an extension.

### Parameters

*   `name` **[string][27]** The name of the extension.

### setInstructions

#### Parameters

*   `instructions` **[string][27]** The instructions of the extension for the AI agent.

### setFunctionSchemas

#### Parameters

*   `functionSchemas` **[array][28]** The function schemas of the extension for the AI agent.

### setFunctions

#### Parameters

*   `functions` **[array][28]** The named functions of the extension.

## Module

Represents a module.

### Parameters

*   `name` &#x20;
*   `type` &#x20;

### setVersion

#### Parameters

*   `version` **[string][27]** The version of the module.

### setDescription

#### Parameters

*   `description` **[string][27]** The description of the module.

### setInstallationGuide

#### Parameters

*   `installationGuide` **[string][27]** The installation guide of the module.

### setEnvironmentVariables

#### Parameters

*   `environmentVariables` **[array][28]** The environment variables of the extension.

### setDockerRepository

#### Parameters

*   `dockerRepository` **[string][27]** The docker repository of the extension.

### setDockerVolumeData

#### Parameters

*   `dockerVolumeData` **[string][27]** The docker volume data of the extension.

## Readme

Represents a readme.

### Parameters

*   `templateUrl` **[string][27]** The template URL.
*   `path` **[string][27]** The path of the readme file.
*   `module` **[Module][9]** The module (e.g. an extension).

## Service

Represents a service.

### Parameters

*   `agentUrls` **[array][28]** The agent URLs.
*   `modules` **([Module][9] | [array][28])** The modules (e.g. an extension).

[1]: #extension

[2]: #parameters

[3]: #setinstructions

[4]: #parameters-1

[5]: #setfunctionschemas

[6]: #parameters-2

[7]: #setfunctions

[8]: #parameters-3

[9]: #module

[10]: #parameters-4

[11]: #setversion

[12]: #parameters-5

[13]: #setdescription

[14]: #parameters-6

[15]: #setinstallationguide

[16]: #parameters-7

[17]: #setenvironmentvariables

[18]: #parameters-8

[19]: #setdockerrepository

[20]: #parameters-9

[21]: #setdockervolumedata

[22]: #parameters-10

[23]: #readme

[24]: #parameters-11

[25]: #service

[26]: #parameters-12

[27]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String

[28]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array
