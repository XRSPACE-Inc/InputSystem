---
uid: input-system-workflows
---

# Input System Workflows

There are multiple ways to use the Input System, however the primary and recommended workflow is to use the **Input Actions** panel in the **Project Settings window** to configure your project-wide Actions and Bindings, and then read the values for those actions in your code using the `InputActions` class.

There are other workflows which can suit more unusual situations, for example you can use the **PlayerInput component** together with Actions and Bindings which adds a further layer of abstraction, allowing you to connect actions to your event handlers without requiring any intermediate code.

You can choose to configure Actions and Bindings in the Editor UI, or you can set up everything through scripting. Or you can take a more direct aproach by omitting the Actions and Bindings altogether and instead use script to directly read the state of devices.

The descriptions below describe these main workflows and link to more detailed description of them.



* [**Configure input in the Editor, and read user actions using the InputActions class**](Workflow-ProjectWideActions)<br/>The primary and recommended workflow for most situations. In this workflow, you use the Input Settings window to configure your project-wide actions and bindings, then read the values for those actions in your code using the `InputActions` class [(read more)](Workflow-ProjectWideActions).<br/><br/>

* [**Configure input in the Editor, use PlayerInput component to handle events**](Workflow-PlayerInput)<br/>This workflow adds an extra layer of abstraction on top of Actions and Bindings configuration, as well as providing features that are useful in multiplayer scenarios such as split-screen or online multiplayer. In addition to using an Actions, you can place the PlayerInput component on to GameObjects to connect Actions to event handlers, removing the need for any intermediary code between the Input System and your input event handler code [(read more)](Workflow-PlayerInput).<br/><br/>

* [**Read user input directly from devices**](Workflow-Direct)<br/>A simplified, script-only approach which is less abstracted, but also less flexible. Your script explicitly references specific device controls (such as "left gamepad stick") and reads the values directly. This is suitable for fast prototyping, or single fixed platform scenarios [(read more)](Workflow-Direct).<br/><br/>

> **Note**: Because the Input System has multiple workflows, the code samples used throughout this documentation also vary, demonstrating techniques using various workflows. For example, some code samples may use the InputActions class, some may reference actions using a string, and some may read input directly from devices.
