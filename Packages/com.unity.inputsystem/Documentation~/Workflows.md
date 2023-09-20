---
uid: input-system-workflows
---

# Input System Workflows

There are multiple ways to use the Input System, however the primary and recommended workflow is to use the **Input Actions** panel in the **Project Settings window** to configure your project-wide Actions and Bindings, and then read the values for those actions in your code using the `InputActions` class.

There are other workflows which can suit more unusual situations, for example you can take a more direct aproach by omitting the Actions and Bindings altogether and instead **directly read the state of controls** on your device.

Or you can use the **PlayerInput component** together with Actions and Bindings which adds a further layer of abstraction, allowing you to connect actions to your event handlers without requiring any intermediate code.

The diagrams on this page show the flow of input from the device to end result in your code, to help you understand the steps involved.



|   |   |
|---|---|
|[**Read project-wide actions using InputActions class**](Workflow-ProjectWideActions.html)<br/>The primary and recommended workflow for most situations. Use the Input Settings window to configure your project-wide Actions and Bindings, then read the values for those actions in your code using the `InputActions` class.<br/><br/>[Read more](Workflow-ActionsAsset.html)|(Image Removed)|
|[**Directly Reading Device States**](Workflow-Direct.html)<br/>A simplified, script-only approach which is less abstracted, but also less flexible. Your script explicitly refers to specific device controls and reads the values directly. Suitable for fast prototyping, or single fixed platform scenarios.<br/><br/>[Read more](Workflow-Direct.html) |![image alt text](Images/Workflow-Direct.svg)|
|[**Using an Actions Asset and a PlayerInput component**](Workflow-PlayerInput.html)<br/><br/>An extra layer of abstraction on top of Actions and Bindings configuration. In addition to using an Actions, you can place the PlayerInput component on to GameObjects to connect actions to event handlers, removing the need for any intermediary code between the Input System and your input event handler code.<br/><br/>NOTE ABOUT MULTIPLAYER HERE

Suitable for situations where you want to reduce the amount of code required to an absolute minimum, such as **asset store** packages.<br/><br/>[Read more](Workflow-PlayerInput.html)|(Image Removed)|

>[!Note]
>Because the Input System has multiple workflows, the code samples used throughout this documentation also vary, demonstrating techniques using various workflows. For example, some code samples may use embedded actions, and others might use an action asset.
