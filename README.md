# Sour Client UI v2 (1.21.11)

## Controls
- **Right Shift** opens the GUI.
- **Left click** toggles a module.
- **Right click** opens module settings.
- **Bind row** inside settings lets you assign a key.

## Commands
- `.help`
- `.modules`
- `.toggle fpsboost`
- `.bind fpsboost rshift`
- `.config save default`
- `.config load default`

## Adding a module
1. Create a class in `src/main/java/com/sourclient/module/impl/...` that extends `Module`.
2. Add settings with `addSetting(...)`.
3. Register it in `ModuleManager#init()`.
4. It will appear in the GUI and config system automatically.

## Safe modules included
- FPS Boost
- FPS Counter
- Watermark
- Appearance / theme settings

## Build
```bash
./gradlew build
```
On Windows:
```bat
gradlew build
```


Author: Tymek24
Minecraft version: 1.21.11
