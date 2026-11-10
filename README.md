
Duplicate titlebar buttons can occur on Zen when using transparent browser mods with DWMBlurGlass or OpenGlass, on Windows 10. 
This mod hides the extra Windows-native titlebar buttons and lets Zen's remain.

### Before
![Before fix](https://raw.githubusercontent.com/landnthrnnn/DUMP/refs/heads/main/GitHub/repos/zen-duplicate-titlebar-fix/before.png)

### After
![After fix](https://raw.githubusercontent.com/landnthrnnn/DUMP/refs/heads/main/GitHub/repos/zen-duplicate-titlebar-fix/after.png
)

## How It Works

- Detects Zen's main browser windows and removes the `WS_SYSMENU` window style, preventing Windows from drawing its native titlebar buttons over Zen's.   
  Also prevents Zen from restoring that style while the mod is active.
- The fix involves removing the native Windows system menu from being used on Zen, normally accessible with `alt + space`
- Only targets `zen.exe`
 