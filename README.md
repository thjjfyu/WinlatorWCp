# 🤖 Winlator Resources 🚧 WIP

## ⚙️ FEX
| Build | Description | Source |
|-------|-------------|:------:|
| [**FEX-Stable**](https://github.com/Arihany/Winlator-Resources/releases/tag/FEX-STABLE) | Stable | <a href="https://github.com/FEX-Emu/FEX">🔗</a> |
| [**FEX-Nightly**](https://github.com/Arihany/Winlator-Resources/releases/tag/FEX-NIGHTLY) | Nightly (YYMMDD) |  |
<br>

## 📦 BOX64
Nightly builds use the YYMMDD filename format
| Build | Description | Source |
|-------|-------------|:------:|
| [**Glibc-Stable**](https://github.com/Arihany/Winlator-Resources/releases/tag/BOX64-STABLE) | Stable | <a href="https://github.com/ptitSeb/box64">🔗</a> |
| [**Glibc-Nightly**](https://github.com/Arihany/Winlator-Resources/releases/tag/BOX64-NIGHTLY) | Nightly |  |
| **Bionic-Stable** | Stable | <a href="https://github.com/ptitSeb/box64">🔗</a> |
| [**Bionic-Nightly**](https://github.com/Arihany/Winlator-Resources/releases/tag/BOX64-BIONIC-NIGHTLY) | Nightly |  |
<br>

## 🧩 DXVK
| Build | Description | Source |
|-------|-------------|:------:|
| [**DXVK**](https://github.com/Arihany/Winlator-Resources/releases/tag/DXVK) | Original source build | <a href="https://github.com/doitsujin/dxvk">🔗</a> |
| [**DXVK-Sarek**](https://github.com/Arihany/Winlator-Resources/releases/tag/DXVK-SAREK) | For low-spec (lower Vulkan support) | <a href="https://github.com/pythonlover02/DXVK-Sarek">🔗</a> |
| [**DXVK-Sarek-Async**](https://github.com/Arihany/Winlator-Resources/releases/tag/DXVK-SAREK-ASYNC) | Async + For low-spec | <a href="https://github.com/pythonlover02/DXVK-Sarek/tree/async">🔗</a> |
| [**DXVK-GPLAsync**](https://github.com/Arihany/Winlator-Resources/releases/tag/DXVK-GPLASYNC) | GPL+Async patch (reduced stutter) | <a href="https://gitlab.com/Ph42oN/dxvk-gplasync">🔗</a> |
| [**DXVK-ARM64EC**](https://github.com/Arihany/Winlator-Resources/releases/tag/DXVK-ARM64EC) | FEX build for performance | <a href="https://wiki.fex-emu.com/index.php/Development:ARM64EC">🔗</a> |
| [**DXVK-GPLAsync-ARM64EC**](https://github.com/Arihany/Winlator-Resources/releases/tag/DXVK-GPLASYNC-ARM64EC) | FEX build + GPL+Async patch | <a href="https://gitlab.com/Ph42oN/dxvk-gplasync">🔗</a><a href="https://wiki.fex-emu.com/index.php/Development:ARM64EC">🔗</a> |
<br>

## 🌌 VKD3D-Proton
| Build | Description | Source |
|-------|-------------|:------:|
| [**VKD3D-Proton**](https://github.com/Arihany/Winlator-Resources/releases/tag/VKD3D-PROTON) | Original source build | <a href="https://github.com/HansKristian-Work/vkd3d-proton">🔗</a> |
| [**VKD3D-Proton-ARM64EC**](https://github.com/Arihany/Winlator-Resources/releases/tag/VKD3D-PROTON-ARM64EC) | FEX build for performance | <a href="https://github.com/HansKristian-Work/vkd3d-proton">🔗</a><a href="https://wiki.fex-emu.com/index.php/Development:ARM64EC">🔗</a> |
<br>

## 🖥️ Runtime Packages
If older Visual C++ versions are required, you may try an AIO package<br>
Some exe may require the official .NET Framework instead of Mono
| Build | Description |
|-------|-------------|
| [**Visual C++ x64**](https://aka.ms/vs/17/release/vc_redist.x64.exe) | 2015–2022 Redistributable |
| [**Visual C++ x86**](https://aka.ms/vs/17/release/vc_redist.x86.exe) | 2015–2022 Redistributable |
| [**Visual C++ ARM64**](https://aka.ms/vs/17/release/vc_redist.arm64.exe) | 2015–2022 Redistributable (arm64ec) |
| [**Wine-Mono**](https://github.com/wine-mono/wine-mono/releases) | .NET runtime for Wine (*.msi) |
| [**Wine-Gecko**](https://dl.winehq.org/wine/wine-gecko/) | HTML engine for Wine (*.msi) |
| [**XNA Framework**](https://download.microsoft.com/download/a/c/2/ac2c903b-e6e8-42c2-9fd7-bebac362a930/xnafx40_redist.msi) | Old indie games runtime |
| [**DirectX (June 2010)**](https://download.microsoft.com/download/8/4/a/84a35bf1-dafe-4ae8-82af-ad2ae20b6b14/directx_Jun2010_redist.exe) | Install ONLY if missing DLL (d3dx9_43.dll, d3dcompiler_43.dll) |
| [**PhysX Legacy**](https://www.nvidia.com/content/DriverDownload-March2009/confirmation.php?url=/Windows/9.13.0604/PhysX-9.13.0604-SystemSoftware-Legacy.msi&lang=us&type=Other) | Install ONLY if a old game requests PhysX DLL |
<br>

## Adrenotools GPU Drivers
## Proton


## ℹ️Notes
- 🚧 It might be that my ignorance broke the build. If that happens, please let me know!
- 🤖 All builds are automatically generated from the latest official source release
- 🔗 Official Box64 configuration can be found [here](https://github.com/ptitSeb/box64/blob/main/system/box64.box64rc)
- ✨ All credit goes to the original creators and those who inspired this work


[ptitSeb](https://github.com/ptitSeb)  
[doitsujin](https://github.com/doitsujin)  
[pythonlover02](https://github.com/pythonlover02)  
[Ph42oN](https://gitlab.com/Ph42oN)  
[HansKristian-Work](https://github.com/HansKristian-Work)  
[brunodev85](https://github.com/brunodev85)  
[coffincolors](https://github.com/coffincolors)  
[Pipetto-crypto](https://github.com/Pipetto-crypto)  
[K11MCH1](https://github.com/K11MCH1)

