<h1 align="center">Winlator WCP Hub</h1>
<br>

<p align="center">
  <img src="./Logo.png" alt="logoo" width="260">
</p>


<h3 align="center">Automated builds, Always up to date</h3>

---

<br>

## ⚙️ FEXCore & Box64
📌 Nightly - YYMMDD
| Type | Build | 📜 |
|:------:|:------:|:------:|
| FEXCore | [**Stable**](https://github.com/Arihany/WinlatorWCPHub/releases/tag/FEX-STABLE) · [**Nightly**](https://github.com/Arihany/WinlatorWCPHub/releases/tag/FEX-NIGHTLY) | <a href="https://github.com/FEX-Emu/FEX">🔗</a> |
| Box64 Glibc | [**Stable**](https://github.com/Arihany/WinlatorWCPHub/releases/tag/BOX64-STABLE) · [**Nightly**](https://github.com/Arihany/WinlatorWCPHub/releases/tag/BOX64-NIGHTLY) | <a href="https://github.com/ptitSeb/box64">🔗</a> |
| Box64 Bionic | [**Nightly**](https://github.com/Arihany/WinlatorWCPHub/releases/tag/BOX64-BIONIC-NIGHTLY)| |

<details>
  <summary>⚡More info</summary>
  
| Type       | Description                                                   |
|:------:|---------------------------------------------------------------|
| **FEXCore**  | Easy to set up, and you can squeeze more performance by pairing it with the arm64ec translation layer.<br>(Games that require box64’s ```STRONGMEM``` might not run well on FEX.) |
| **Box64** | Setup is more involved, but it generally runs more games than FEX.<br>(Some picky titles may also run more smoothly.) |

I recommend FEX by default. It’s easy to set up and usually just works.<br>
Basic Box64 settings for unity games: ```STRONGMEM=1+ CALLRET=0 WEAKBARRIER=0~1```
</details>
</details>
<br>

## 🧩 DXVK
| Build | 📜 |
|-------|:------:|
| [**DXVK**](https://github.com/Arihany/WinlatorWCPHub/releases/tag/DXVK) |  <a href="https://github.com/doitsujin/dxvk">🔗</a> |
| [**DXVK-sarek**](https://github.com/Arihany/WinlatorWCPHub/releases/tag/DXVK-SAREK) |  <a href="https://github.com/pythonlover02/DXVK-Sarek">🔗</a> |
| [**DXVK-sarek-async**](https://github.com/Arihany/WinlatorWCPHub/releases/tag/DXVK-SAREK-ASYNC) |   |
| [**DXVK-sarek-async-arm64ec**](https://github.com/Arihany/WinlatorWCPHub/releases/tag/DXVK-SAREK-ASYNC-ARM64EC) |   |
| [**DXVK-gplasync**](https://github.com/Arihany/WinlatorWCPHub/releases/tag/DXVK-GPLASYNC) |  <a href="https://gitlab.com/Ph42oN/dxvk-gplasync">🔗</a> |
| [**DXVK-arm64ec**](https://github.com/Arihany/WinlatorWCPHub/releases/tag/DXVK-ARM64EC) |   |
| [**DXVK-gplasync-arm64ec**](https://github.com/Arihany/WinlatorWCPHub/releases/tag/DXVK-GPLASYNC-ARM64EC) |   |

<details>
  <summary>⚡More info</summary>
  
| Type       | Description                                                   |
|:------:|---------------------------------------------------------------|
| **sarek**    | Provides backports for old GPUs that don’t support Vulkan 1.3.<br>May run faster on older devices. |
| **gplasync** | Reduces stuttering by rendering frames before shader compilation.<br>Possible graphics glitches. |
| **arm64ec**  | Boosts performance in 64-bit games. **Use only with FEX.**<br>(32-bit = same as standard DXVK.) |

Try Sarek first. if you run into issues, try another version.<br>
Newer versions don’t always mean better performance.
</details>
<br>

## 🌌 VKD3D-Proton
| Build | 📜 |
|-------|:------:|
| [**VKD3D-proton**](https://github.com/Arihany/WinlatorWCPHub/releases/tag/VKD3D-PROTON) |  <a href="https://github.com/HansKristian-Work/vkd3d-proton">🔗</a> |
| [**VKD3D-proton-arm64ec**](https://github.com/Arihany/WinlatorWCPHub/releases/tag/VKD3D-PROTON-ARM64EC) |   |

<details>
  <summary>⚡More info</summary>
  
| Type       | Description                                                   |
|:------:|---------------------------------------------------------------|
| **arm64ec**  | Boosts performance in 64-bit games. **Use only with FEX.**<br>(32-bit = same as standard DXVK.) |

</details>
<br>

## 📦 Runtime Packages (official)
📌 If older VC++ is needed, try an AIO package. <br>
📌 May require the official .NET Framework instead of Mono.
| Package | Description |
|-------|-------------|
| [**Visual C++ x64**](https://aka.ms/vs/17/release/vc_redist.x64.exe) | 2015–2022 Redistributable |
| [**Visual C++ x86**](https://aka.ms/vs/17/release/vc_redist.x86.exe) | 2015–2022 Redistributable |
| [**Visual C++ ARM64**](https://aka.ms/vs/17/release/vc_redist.arm64.exe) | 2015–2022 Redistributable |
| [**Wine-Mono**](https://github.com/wine-mono/wine-mono/releases) | .NET runtime for Wine (*.msi) |
| [**Wine-Gecko**](https://dl.winehq.org/wine/wine-gecko/) | HTML engine for Wine (*.msi) |
| [**XNA Framework**](https://download.microsoft.com/download/a/c/2/ac2c903b-e6e8-42c2-9fd7-bebac362a930/xnafx40_redist.msi) | Old indie games runtime |
| [**DirectX (June 2010)**](https://download.microsoft.com/download/8/4/a/84a35bf1-dafe-4ae8-82af-ad2ae20b6b14/directx_Jun2010_redist.exe) | Install ONLY if missing DLL (d3dx9_43.dll...) |
| [**PhysX Legacy**](https://www.nvidia.com/content/DriverDownload-March2009/confirmation.php?url=/Windows/9.13.0604/PhysX-9.13.0604-SystemSoftware-Legacy.msi&lang=us&type=Other) | Install ONLY if a old game requests PhysX DLL |
<br>


## ✨...

<br><br>

---

<h3 align="center">All credit to the original creators. Big thanks to everyone who inspired this.</h3><p align="center">
<h3 align="center">
  
[bylaws](https://github.com/bylaws)<br>
[ptitSeb](https://github.com/ptitSeb)  
[doitsujin](https://github.com/doitsujin)  
[pythonlover02](https://github.com/pythonlover02)  
[Ph42oN](https://gitlab.com/Ph42oN)  
[HansKristian-Work](https://github.com/HansKristian-Work)  
[brunodev85](https://github.com/brunodev85)  
[coffincolors](https://github.com/coffincolors)  
[Pipetto-crypto](https://github.com/Pipetto-crypto)  
[K11MCH1](https://github.com/K11MCH1)

</h3><p align="center">

