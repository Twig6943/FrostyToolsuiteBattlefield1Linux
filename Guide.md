# How to use this thing

1.Download the binaries from the [releases section](https://github.com/twig6943/FrostyToolsuiteBF1linux/releases)

2.Add the following dlloverrides to your wineprefix via `winecfg` & environment variable :

### Winecfg
```sh
winmm
dinput8
marne
```

(Should be set to `native,builtin`)

### Environment variable

```sh
WINEDLLOVERRIDES=dinput8=n,b;Marne=n,b;winmm=n,b;
```

3.Run `taskmgr` inside the wineprefix

4.Select the .exe for the fmm bf1 linux build

5.Load & apply the mods you want

6.Add the `GAME_DATA_DIR` and the path to your modpack (for most people its just `C:\Program Files\EA Games\Battlefield 1\ModData\Default`) 

(You need to get the path for that folder using a wine/windows explorer)

![](/assets/01.png)

7.Launch the game and everything should work.

