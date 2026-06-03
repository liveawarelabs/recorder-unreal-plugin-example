# Unreal Engine Example Project for Live Aware Labs Recorder Plugin

This repo contains sample Unreal Engine projects to verify and demonstrate usage of the LiveAwareRecorder plugin.

> **NOTE:** This repo uses Git LFS. Do not download it as a zip file from GitHub.

## Example Projects

| Folder | Unreal Engine version | Status |
| --- | --- | --- |
| `RecorderPluginExampl_UE5.7` | Unreal Engine 5.7 | Current validated example |
| `RecorderPluginExampl` | Unreal Engine 5.0.3+ | Legacy example |

Use the example folder that matches your Unreal Engine version. The UE 5.7 example is the recommended starting point for current testing.

## Prerequisites

- Windows 10+
- Unreal Engine matching the selected example folder
- Microsoft Visual Studio with C++ game development tools
- Windows SDK
- .NET Framework 4.8 Developer Pack / SDK
- Enough free disk space for Unreal build artifacts; 20 GB or more is recommended

## Plugin Setup

Download and install the [latest plugin release](https://liveawarenexus.sfo3.cdn.digitaloceanspaces.com/LiveAwareSDK/Unreal/LiveAwareUnrealPlugin.zip).

For source checkouts, copy the plugin into the selected example project's `Plugins/LiveAwareRecorder` folder before generating project files or opening the `.uproject`.

Customer release archives may already include the plugin staged in `Plugins/LiveAwareRecorder`.

## Generated Files

Do not commit generated Unreal or Visual Studio output such as `Binaries`, `Intermediate`, `.vs`, `Saved`, packaged builds, or generated solution files.
