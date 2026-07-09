# VC2SAMP / VC2OMP
[![License](https://img.shields.io/badge/license-GPLv3-blue.svg)](LICENSE)

This is a conversion of Vice City to SA-MP 0.3DL, as well as OMP.

## Download Project .ZIP
Check the release page for a zip containing the project.

## Requeriments
[Streamer](http://forum.sa-mp.com/showthread.php?t=102865) by Incognito

[ZCMD](http://forum.sa-mp.com/showthread.php?t=91354) by Zeex (OPTIONAL)

[foreach](http://forum.sa-mp.com/showthread.php?t=570868) (optional) by Y_Less (OPTIONAL)

## Installation in SAMP
1. Download the vice_city.pwn and put it in your filterscript folder, then compile with 0.3DL includes if you wish.
2. Download the models and put "vc4samp" in models folders.
3. Put vice_city in the filterscript line in server.cfg or use /rcon loadfs vice_city
4. Use command /gotovc - enjoy the city.

## Configuration in open.mp

Open your `config.json` file and locate the `"pawn"` section.

Add the filterscript to the `"side_scripts"` array.

> **Note:** Do **not** include the `.amx` extension.

### Example

```json
{
    "pawn": {
        "legacy_plugins": [
            "streamer",
            "sscanf"
        ],
        "main_scripts": [
            "your_gamemode 1"
        ],
        "side_scripts": [
            "filterscripts/vice_city"
        ]
    }
}
```

After saving `config.json`, restart your open.mp server. The VC2OMP filterscript will be loaded automatically on startup.
