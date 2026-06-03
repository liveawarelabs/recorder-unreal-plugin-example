# Live Aware Recorder Unreal Engine Example

This repository contains Unreal Engine sample projects for testing the LiveAwareRecorder plugin.

Use these examples to confirm the plugin loads, explore the included Blueprint widgets, and verify basic recorder integration in an Unreal project.

> **Important:** This repository uses Git LFS for Unreal assets. Clone it with Git instead of downloading the GitHub source zip.

## Choose An Example

| Folder | Unreal Engine version | Recommendation |
| --- | --- | --- |
| `RecorderPluginExampl_UE5.7` | Unreal Engine 5.7 | Recommended for new testing |
| `RecorderPluginExampl` | Unreal Engine 5.0.3+ | Legacy example |

Use the folder that matches your installed Unreal Engine version. If you are starting fresh, use `RecorderPluginExampl_UE5.7`.

## Requirements

- Windows 10 or newer
- Unreal Engine matching the selected example
- Visual Studio with C++ game development tools
- Windows SDK
- .NET Framework 4.8 Developer Pack / SDK
- At least 20 GB of free disk space for Unreal-generated build files

## Quick Start

1. Clone this repository with Git LFS enabled.
2. Download the latest LiveAwareRecorder Unreal plugin:
   https://liveawarenexus.sfo3.cdn.digitaloceanspaces.com/LiveAwareSDK/Unreal/LiveAwareUnrealPlugin.zip
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

## Troubleshooting

- If Unreal reports missing plugin files, confirm the plugin is extracted to `Plugins/LiveAwareRecorder` inside the selected example folder.
- If the editor build fails with a .NET Framework SDK error, install the .NET Framework 4.8 Developer Pack / SDK.
- If the build fails while Live Coding is active, close Unreal Editor and the Live Coding console, then build again.
- If compilation fails with disk-space errors, free additional space and delete generated `Intermediate` and `Binaries` folders before retrying.

## Generated Files

Unreal and Visual Studio generate large local build files. Do not commit or share generated folders such as `Binaries`, `Intermediate`, `.vs`, `Saved`, packaged builds, or generated solution files.
