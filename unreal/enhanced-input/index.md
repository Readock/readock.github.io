---
layout: page
title: Enhanced Input
description: Unreal plugin that is replacing the old input system
categories: [Unreal]
breadcrumb_path: "Unreal"
searchable: true
author: felix
toc: true
---

Unreal plugin to replace the old input method. 

## Input Actions

Input Actions are the connection between the system and the code. 

> Create a new action for diffrent contexts. Eg. `SkipCutsceneAction` and `SkipDialogAction` are better
then just one `SkipAction` because then the context does not get handled by the Input system and you will need custom code to check what to skip
{: .prompt-tip }

## Input Mapping Contexts

Maps user inputs to Actions and can be dynamically added, removed, or prioritized

## Trigger States

* Triggered
    * The action has been triggered! This means that it has completed the evaluation of all trigger requirements. For example, a "Press and Release" trigger is sent when the user releases the key.
* Started
    * An event has occurred that has begun trigger evaluation. For example, the first press of a "Double tap" trigger will call the "Started" state once. 
* Ongoing
    * The trigger is still being processed. For example, a "Press and hold" action is ongoing while the user is holding down the button before the specified duration is reached. Depending on the triggers, this event fire every tick that the action is being evaluated once it receives an input value.
* Completed
    * The trigger evaluation process is completed. 
* Canceled
    * The triggering has been canceled. For example, a user lets go of a button before a "Press and Hold" action can be triggered.

> Its probably good to use the `triggered` event as the default option to implement behaviour for actions (Eg. using `Started` and then adding triggers might produce unexpected behaviour)
{: .prompt-tip }


## Subscribe to Actions

To add an input action listener in blueprints you can right click in the blueprints event graph and type in the name of your input action data asset. 

> If you want to use Input Actions in an Bluepring Actor you need to call `EnableInput` to be able to use Action Events 
{: .prompt-tip }


## Debugging

{: file='console'}
```c++
showdebug enhancedinput
```

## Resources

A great overview can be found here: [**Enhanced Input in UE5**](https://dev.epicgames.com/community/learning/tutorials/eD13/unreal-engine-enhanced-input-in-ue5)