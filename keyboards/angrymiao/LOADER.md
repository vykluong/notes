# AngryMiao (Loader) Installer Package
Describes how to open loader without installer

## Expand PKG
Extract downloaded file compressed (e.g., `.zip`) and expand `.pkg` into directory (e.g., `AngryMiao`)
```sh
> pkgutil --expand-full AngryMiaoKeyboard_Mac-20220402-1.0.7.pkg AngryMiao
```

## Run AngryMiao.app
Requires [tree](https://github.com/Old-Man-Programmer/tree)
```sh
> tree AngryMiao --level 4
AngryMiao
.
├── AngryMiaoKeyboard_Mac.pkg
│   ├── Bom
│   ├── PackageInfo
│   ├── Payload
│   │    ├── Applications
│   │    │  └── AngryMiao.app
│   │    ├── Library
│   │    │  └── LaunchAgents
│   │    └── usr
│   │        └── local
│   └── Scripts
├── Distribution
└── Resources
    ├── en.lproj
    │  └── Localizable.strings
    └── zh_CN.lproj
        ├── license.rtfd
        ├── readme.rtfd
        └── welcome.rtfd
```

## Clean up
```sh
> rm -rf AngryMiao*
```
