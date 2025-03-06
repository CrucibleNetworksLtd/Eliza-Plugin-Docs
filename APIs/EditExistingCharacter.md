---
title: EditExistingCharacter
layout: default
parent: Home
---

![](EditExistingCharacter.png)

Edits an existing Eliza agent on the server, replacing its character with the given character. You must supply an a Character struct with the "id" being the same as the id of the character you want to edit on the eliza server.

# Inputs

| - | - | - |
|Type|Name|Description|
|FString|AgentId|The AgentId of the agent you want to replace the character of.|
|FAgentDetailsCharacter|AgentCharacter|The character struct that the agent will use. You must supply an a Character struct with the "id" being the same as the id of the character you want to edit on the eliza server.|
|UElizaInstance\*|ElizaInstance|The Eliza instance that we should be communicating with. This can either be a ElizaInstance game asset created in the content browser, or created on the fly with the CreateElizaInstance method.|

# Outputs

| - | - | - |
|Type|Name|Description|
|bool|Success|If this method was a HTTP success, usable as a quick check to see if it immediately failed.|

# C++
Module: `Eliza`
include: `#include "EditExistingCharacter.h"`

`UEditExistingCharacter::EditExistingCharacter(FString AgentId, FAgentDetailsCharacter AgentCharacter, UElizaInstance* ElizaInstance)` - instantiates this async method.
`Activate()` - Activates this async method.
In C++, the outputs of the async function can be acted upon by binding to the event delegate "`OnEditExistingCharacterCompleted`".
