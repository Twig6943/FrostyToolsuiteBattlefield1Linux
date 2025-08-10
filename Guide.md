# How to use this thing

1.Download the binaries from the [releases section](https://github.com/Twig6943/FrostyToolsuiteBattlefieldLinux/releases)

2.Add the following dlloverrides to your wineprefix via `winecfg` & environment variable :

## Winecfg

### Marne

```sh
dinput8
marne
winmm
```

# Tonga

```sh
dinput8
tonga
winmm
```

(Should be set to `native,builtin`)

## Environment variable

### Marne

```sh
WINEDLLOVERRIDES=dinput8=n,b;Marne=n,b;winmm=n,b
```

### Tonga

```sh
WINEDLLOVERRIDES=dinput8=n,b;Tonga=n,b;crypthook=n,b;winmm=n,b
```

3.Run `taskmgr` inside the wineprefix

4.Select the FrostyModManager.exe

5.Load & apply the mods you want

6.Add the `GAME_DATA_DIR` and the path to your modpack (for most people its just `C:\Program Files\EA Games\Battlefield 1\ModData\Default`) 

(You need to get the path for that folder using a wine/windows explorer)

![](/assets/01.png)

7.Launch the game and everything should work.
