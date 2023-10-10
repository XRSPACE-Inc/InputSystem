---
uid: input-system-workflows
---

# Input System Workflows

There are multiple ways to use the Input System, however the primary and recommended workflow is to use the **Input Actions** panel in the **Project Settings window** to configure your project-wide Actions and Bindings, and then read the values for those actions in your code using the `InputActions` class.

There are other workflows which can suit more unusual situations, for example you can use the **PlayerInput component** together with Actions and Bindings which adds a further layer of abstraction, allowing you to connect actions to your event handlers without requiring any intermediate code, or you can take a more direct aproach by omitting the Actions and Bindings altogether and instead directly read the state of devices.

The descriptions below describe these main workflows and link to more detailed documentation.



* [**Read user actions using InputActions class**](Workflow-ProjectWideActions.html)<br/>The primary and recommended workflow for most situations. Use the Input Settings window to configure your project-wide actions and bindings, then read the values for those actions in your code using the `InputActions` class. [Read more](Workflow-ProjectWideActions.html),<br/><br/>
* [**Using an Actions and a PlayerInput component**](Workflow-PlayerInput.html)<br/>This workflow adds an extra layer of abstraction on top of Actions and Bindings configuration, and provides features that are useful in multiplayer scenarios such as split-screen or online multiplayer. In addition to using an Actions, you can place the PlayerInput component on to GameObjects to connect Actions to event handlers, removing the need for any intermediary code between the Input System and your input event handler code. [Read more](Workflow-PlayerInput.html).<br/><br/>
* [**Read user input directly from devices**](Workflow-Direct.html)<br/>A simplified, script-only approach which is less abstracted, but also less flexible. Your script explicitly references specific device controls (such as "left gamepad stick") and reads the values directly. This is suitable for fast prototyping, or single fixed platform scenarios. [Read more](Workflow-Direct.html).<br/><br/>

> **Note**: Because the Input System has multiple workflows, the code samples used throughout this documentation also vary, demonstrating techniques using various workflows. For example, some code samples may use embedded actions, and others might use an action asset.
