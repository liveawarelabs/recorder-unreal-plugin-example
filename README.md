# Live Aware Recorder Unreal Engine Example

This repository contains Unreal Engine sample projects for testing the LiveAwareRecorder plugin.

Use these examples to confirm the plugin loads, explore the included Blueprint widgets, and verify basic recorder integration in an Unreal project.

> **Important:** This repository uses Git LFS for Unreal assets. Clone it with Git instead of downloading the GitHub source zip.

## Choose An Example

| Folder | Unreal Engine version | Recommendation |
| --- | --- | --- |
| `RecorderPluginExampl_UE5.7` | Unreal Engine 5.7 | Currently validated and recommended |
| `RecorderPluginExampl` | Unreal Engine 5.0.3+ | Legacy example, not currently validated |

Use `RecorderPluginExampl_UE5.7` for new testing. The older `RecorderPluginExampl` folder is retained for legacy Unreal Engine projects, but it has not been validated with the current plugin release.

## Requirements

- Windows 10 or newer
- Unreal Engine matching the selected example
- Visual Studio 2022 or newer with C++ game development tools
- .NET Framework 4.8 Developer Pack / SDK for Unreal editor builds

## Quick Start

1. Clone this repository with Git LFS enabled.
2. Download the [latest plugin release](https://liveawarenexus.sfo3.cdn.digitaloceanspaces.com/LiveAwareSDK/Unreal/LiveAwareUnrealPlugin.zip).
3. Extract the plugin into the selected example project so the folder exists at:
   `Plugins/LiveAwareRecorder`
4. Right-click the selected `.uproject` file and choose **Generate Visual Studio project files**.
5. Open the `.uproject` in Unreal Engine.
6. When prompted, allow Unreal to rebuild project modules.

For UE 5.7, open:

```text
RecorderPluginExampl_UE5.7/RecorderPluginExampl.uproject
```

## Building Manually

If Unreal cannot rebuild modules automatically, build from a Developer PowerShell or terminal:

```powershell
& 'C:\Program Files\Epic Games\UE_5.7\Engine\Build\BatchFiles\Build.bat' RecorderPluginExamplEditor Win64 Development -Project="<repo>\RecorderPluginExampl_UE5.7\RecorderPluginExampl.uproject" -WaitMutex -NoHotReload
```

Replace `<repo>` with the path to this repository.
