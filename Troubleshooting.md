<h1 align="center">Troubleshooting & some info...</h1>
<h3 align="center">⚠️WIP</h3><br><br>

## 📥 How to install
**WCP: Menu → Contents → Install Content**<br><br>

**Driver: Menu → Adrenotools GPU Drivers → Install Drivers**
<br>

---

<br><br><br>

## General

- To resolve issues, start by understanding your game. Look up the game’s engine and common known problems here: [PCGW](https://www.pcgamingwiki.com/wiki/Home).
- Since we’re running on Wine too, browsing Wine(proton)-related forums often yields quick fixes for lots of issues.

## Container
- Some old games only work properly if all services are loaded. (Edit Container → Advanced → System → Load all sevices)
- Some games need to be on the C: drive to launch correctly or to eliminate loading issues and stuttering.
- If there’s a hook DLL, set an environment variable: ```WINEDLLOVERRIDES="name.dll=n,b"```.
- Capping processor affinity can resolve stutter in some games.

## Controller
- Controller dead? Adjust XInput/DInput detection (old games use DInput)
- SDL2 issue? Try this: ```SDL_JOYSTICK_WGI = 0``` ```SDL_XINPUT_ENABLED=1``` ```SDL_JOYSTICK_RAWINPUT=0``` ```SDL_JOYSTICK_HIDAPI=1``` ```SDL_DIRECTINPUT_ENABLED=0``` ```SDL_JOYSTICK_ALLOW_BACKGROUND_EVENTS=1``` ```SDL_HINT_FORCE_RAISEWINDOW=0``` ```SDL_ALLOW_TOPMOST=0``` ```SDL_MOUSE_FOCUS_CLICKTHROUGH=1```
- Best controller support right now: Winlator CMod.

## Box64

- **Regular stuttering** usually means your Box64 settings are too aggressive.
- Unity games are generally more stable when run with Box64.
- Basic Box64 settings for unity games: ```STRONGMEM=1+``` ```CALLRET=0``` ```WEAKBARRIER=0~1```
- ```WEAKBARRIER``` can mitigate the performance hit from ```STRONGMEM```, but regressions or crashes have been reported depending on the build/version/game. If issues occur, set it to ```0```.
- You can find the official Box64 settings [here](https://github.com/ptitSeb/box64/blob/main/system/box64.box64rc)

## FEX
- Games that require box64’s ```STRONGMEM``` might not run well on FEX.

## DXVK

- Newer versions don’t always mean better performance.
- If you encounter rendering issues, try a newer build or revert to the standard DXVK.
- If the game has a built-in frame limiter, use that. In some cases, ```DXVK_FRAME_RATE``` can introduce stutter.
- 2.3.1–2.4.1 are pretty stable overall, but some games still throw the occasional graphics glitch. (Common in UE4(5) games.)
- Games that precompile shaders can cause high load and stutter, wait for compilation to finish and monitor with ```DXVK_HUD=compiler```.

## VKD3D

- If it isn’t required, **leave the VKD3D feature level at its default**. Forcing a higher feature level can trigger different code paths and extra shader compilation, which may lead to stutter.
- You can limit the frame rate using: ```DXVK_FRAME_RATE``` or ```VKD3D_FRAME_RATE```

## Runtime Package

- If Visual C++ errors persist in an ARM64EC container, install ```Visual C++ ARM64```
- If older VC++ is needed, try an [**AIO package**](https://github.com/abbodi1406/vcredist). <br>
- May require the official [**.NET Framework**](https://dotnet.microsoft.com/ko-kr/download/dotnet-framework) instead of Mono.

## Wine/Proton

- Don’t waste time chasing Wine/Proton hoping for fixes or some miracle improvement.


