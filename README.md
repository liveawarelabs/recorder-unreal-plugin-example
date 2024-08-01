# Unreal Engin Example Project for Live Aware Labs Recorder Plugin

This is the sample Unreal Engine project to verify and demonstrate usage of LiveAwareRecorder plugin.
> **_NOTE:_**  This repo uses LFS, don't download it as a zip file from github.

## Prerequisites
- Windows 10+
- Unreal Engine 5.0.3+
- Microsoft Visual Studio 2022
- VS Game Development with C++

## Quick Start
Download and install [latest plugin release](https://liveawarenexus.sfo3.cdn.digitaloceanspaces.com/LiveAwareSDK/Unreal/LiveAwareUnrealPlugin.zip)

## Known Issues
### "cannot convert from 'const From *' to 'TStringConversion<TStringConvert<From,To>,128>'" UE 5.0.3
- Install VS "MSVC v143 - VS 2022 C++ x64/x86 build tools (v14.38-17.8)"
- Replace %APPDATA%\Unreal Engine\UnrealBuildTool\BuildConfiguration.xml file content with
```xml
<?xml version="1.0" encoding="utf-8"?>
    <Configuration xmlns="https://www.unrealengine.com/BuildConfiguration">
      <WindowsPlatform>
        <CompilerVersion>14.38.33130</CompilerVersion>
      </WindowsPlatform>
    </Configuration>
```
- Regenerate Visual Studio solution file for the project
