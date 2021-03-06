# HEMTT

[![Download](https://img.shields.io/badge/download-latest-orange.svg?style=flat)](https://github.com/BrettMayson/HEMTT/releases/latest)
[![Documentation](https://img.shields.io/badge/docs-read-informational.svg)](https://brettmayson.github.io/HEMTT/#/)
[![Travis CI](https://img.shields.io/travis/synixebrett/HEMTT.svg?logo=travis&style=flat)](https://travis-ci.org/synixebrett/HEMTT)
[![AppVeyor CI](https://img.shields.io/appveyor/ci/synixebrett/HEMTT.svg?logo=appveyor&style=flat)](https://ci.appveyor.com/project/synixebrett/HEMTT)  
[![Discord](https://img.shields.io/badge/discord-7289DA)](https://discord.gg/VcDf42t)
[![Chat](https://slackin.ace3mod.com/badge.svg?style=flat&label=ACE3%20Slack%20%23tools)](https://slackin.ace3mod.com)

Build System for Arma 3 powered by [armake2](https://github.com/KoffeinFlummi/armake2) for Linux and Windows - Heavy Expanded Mobility Tactical Truck for Arma 3 mods. HEMTT focuses on CBA and ACE3 standards while providing project configurability and additional utilities.

Read the [documentation](https://brettmayson.github.io/HEMTT) to learn more about it and reference the example project [HEMTT-Example](https://github.com/BrettMayson/HEMTT-Example) to see it in action.


## Using HEMTT

HEMTT is a CLI tool that must be called from the root of your project. HEMTT needs to be placed in the project root and called with `./hemtt` on Linux or `hemtt.exe` on Windows. You can install HEMTT system wide on Windows by using `setup.exe` in the download.

Below is just a showcase, read the [documentation](https://brettmayson.github.io/HEMTT) to learn about more features and reasonings.

### Creating a HEMTT Project

You can either create a brand new Arma 3 mod by using `hemtt create` while in an empty directory or use `hemtt init` while in an existing mod folder to create a `hemtt.json` file. The `hemtt.json` file keeps track various properties of your project.

### Creating a new addon

To add an additional addon (also called component) to your project with all the skeleton files you need, use `hemtt addon [name]`

### Building

You can create a build using `hemtt build` or a release build using `hemtt build --release`.

Any non-addon files you want to be included in the `releases` folder must be included in the `files` propertly in `hemtt.json`.

HEMTT currently uses `addons/main/script_version.hpp` to get version information when doing a release build.


## Download

HEMTT is available for Linux and Windows via [GitHub Releases](https://github.com/BrettMayson/HEMTT/releases/latest).
- Most Windows users will want to use `x86_64-pc-windows-msvc`
- Most Linux users will want to use `x86_64-unknown-linux-gnu`

### Other install methods
##### Via Scoop (unofficial) - Windows
[Scoop](https://scoop.sh/) users can download and install the latest version release by installing the `hemtt` package:
```
scoop bucket add Arma3Tools https://github.com/ColdEvul/arma3-scoop-bucket.git
scoop install hemtt
```
To update HEMTT using Scoop, run the following:
```
scoop update hemtt
```
If you have any issues when installing/updating the package report the same on the [bucket issues page](https://github.com/ColdEvul/arma3-scoop-bucket/issues).

## Contributing

HEMTT is entirely open-source and all contributions are welcome. Check out the [issue list](https://github.com/BrettMayson/HEMTT/issues) and open [pull requests](https://github.com/BrettMayson/HEMTT/pulls)! All submitted code to HEMTT is assumed to be [licensed under GPLv3](https://github.com/BrettMayson/HEMTT/blob/master/LICENSE).

Ideas and discussions are welcome, author and other contributors can be reached on [ACE3 Slack](https://slackin.ace3mod.com) in channel `#tools`. Feel free to join, ask questions or share ideas!

### Thanks

- [KoffeinFlummi](https://github.com/KoffeinFlummi) for [armake2](https://github.com/KoffeinFlummi/armake2) and permission to use his code.
