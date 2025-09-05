<h1 align="center">Troubleshooting & some info...</h1>
<h3 align="center">⚠️WIP</h3><br><br>

## General

- Since we’re running on Wine too, browsing Wine(proton)-related forums often yields quick fixes for lots of issues.
- You can find a game’s traits and common issues on [PCGW](https://www.pcgamingwiki.com/wiki/Home).

## Container
- Some old games only work properly if all services are loaded.<br>(Edit Container → Advanced → System → Load all sevices)
- Some old games need to be on the C: drive to launch correctly or to eliminate loading issues and stuttering.
- If there’s a hook DLL, set an environment variable: ```WINEDLLOVERRIDES="name.dll=n,b"```.
- Capping processor affinity can resolve stutter in some setups.

## Controller
- Controller dead? Adjust XInput/DInput detection (old games use DInput)
- SDL2 issue? Try this: ```SDL_JOYSTICK_WGI = 0``` ```SDL_XINPUT_ENABLED=1``` ```SDL_JOYSTICK_RAWINPUT=0``` ```SDL_JOYSTICK_HIDAPI=1``` ```SDL_DIRECTINPUT_ENABLED=0``` ```SDL_JOYSTICK_ALLOW_BACKGROUND_EVENTS=1``` ```SDL_HINT_FORCE_RAISEWINDOW=0``` ```SDL_ALLOW_TOPMOST=0``` ```SDL_MOUSE_FOCUS_CLICKTHROUGH=1```
- Best controller support right now: Winlator CMod.

## Box64

- **Regular stuttering** usually means your Box64 settings are too aggressive.
- Unity games generally run well with this: ```STRONGMEM=1+``` ```CALLRET=0``` ```WEAKBARRIER=0~1```
- ```WEAKBARRIER``` generally reduces the performance hit caused by ```STRONGMEM```. However, some sensitive games may still fail to run with ```WEAKBARRIER=1```.
- You can find the official Box64 settings [here](https://github.com/ptitSeb/box64/blob/main/system/box64.box64rc)

## FEX
- Games that require box64’s ```STRONGMEM``` might not run well on FEX.

## DXVK

- DXVK 2.3.1–2.4.1 are pretty stable overall, but some games still throw the occasional graphics glitch. (Common in UE5 games.)
- Games that precompile shaders can cause high load and stutter, wait for compilation to finish and monitor with ```DXVK_HUD=compiler```.

## Wine/Proton

- Don’t waste time chasing Wine/Proton hoping for fixes or some miracle improvement. The folks building Winlator and its forks know their stuff. if they haven’t pulled in a newer version, it’s because it isn’t worth it right now.



