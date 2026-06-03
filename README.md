# Live Aware Recorder Unreal Engine Example

This repository contains an Unreal Engine 5.7 sample project for testing the LiveAwareRecorder plugin.

Use this example to confirm the plugin loads, explore the included Blueprint widgets, and verify basic recorder integration in an Unreal project.

> **Important:** This repository uses Git LFS for Unreal assets. Clone it with Git instead of downloading the GitHub source zip.

## Requirements

- Windows 10 or newer
- Unreal Engine 5.7
- Visual Studio 2022 or newer with C++ game development tools
- .NET Framework 4.8 Developer Pack / SDK for Unreal editor builds

## Quick Start

1. Clone this repository with Git LFS enabled.
2. Download the [latest plugin release](https://liveawarenexus.sfo3.cdn.digitaloceanspaces.com/LiveAwareSDK/Unreal/LiveAwareUnrealPlugin.zip).
3. Extract the plugin into the example project so the folder exists at:
   `RecorderPluginExampl_UE5.7/Plugins/LiveAwareRecorder`
4. Right-click `RecorderPluginExampl_UE5.7/RecorderPluginExampl.uproject` and choose **Generate Visual Studio project files**.
5. Open the `.uproject` in Unreal Engine.
6. When prompted, allow Unreal to rebuild project modules.

Open:

```text
RecorderPluginExampl_UE5.7/RecorderPluginExampl.uproject
```
