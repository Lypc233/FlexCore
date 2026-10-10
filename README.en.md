<div align="center">

<img src="assets/flexcore.png" alt="FlexCore" width="64" height="64">

# FlexCore

A CPU core scheduling tool for Windows gaming.

[简体中文](README.md) · **English**

<p>
  <img src="https://img.shields.io/badge/Windows-x64-0078D4?style=flat-square" alt="Windows x64">
  <a href="https://github.com/Lypc233/FlexCore/releases/latest"><img src="https://img.shields.io/github/v/release/Lypc233/FlexCore?style=flat-square&amp;color=E62B35&amp;label=Release" alt="Latest release"></a>
</p>

[Download](https://github.com/Lypc233/FlexCore/releases/latest) · [Quark mirror](https://pan.quark.cn/s/fb393ac897ea) · [Report an issue](https://github.com/Lypc233/FlexCore/issues)

</div>

## Features

FlexCore lets you assign CPU cores to games and background apps, save scheduling rules for each process, and keep those rules active while running in the system tray.

| Feature | What it does |
| :--- | :--- |
| **Core assignment** | View running processes and your CPU layout. Select cores by CCD or performance / efficiency core type where available. |
| **Game scheduling** | V1–V8 modes with preferred cores and affinity enforcement. V8 “双星” supports dual primary-core scheduling. |
| **Background apps** | Group background processes and set their core range, CPU, memory, and I/O priorities together. |
| **Saved rules** | Apply settings automatically when a matching game process runs. Enable or disable rules at any time. |
| **Core isolation** | System core isolation takes effect after a restart. Dynamic core isolation (Pro) works without restarting Windows. |
| **Win32 scheduling** | Adjust foreground scheduling preferences using presets or a custom value, with a restore option. |

Basic scheduling features are free. **Pro** adds V9 “揽月” and dynamic core isolation. Activation is available in the app and requires an internet connection the first time. Restart FlexCore after activation; everyday use works offline.

## Getting started

The page names below match the app's Chinese interface.

1. **Download and run**: Download the `.exe` under **Assets** on the [latest release](https://github.com/Lypc233/FlexCore/releases/latest) and allow the administrator prompt. The Quark mirror above is also available; no extraction code is needed.
2. **Find your game**: Start the game, then find its actual process under **核心分配 → 进程管理** (Core assignment → Process management). Check the game's `.exe` name.
3. **Set up a rule**: Select cores in **核心布局** (Core layout), then check the target process and scheduling mode in **调度规则** (Scheduling rules) and save. Start with the default priorities and adjust as needed.
4. **Play**: Check that the rule is enabled and applied. Keep FlexCore running; scheduling continues when the app is in the system tray.

Results vary by CPU, Windows version, and game. Change one setting at a time and compare frame times and responsiveness in the same scene.

## FAQ

<details>
<summary><b>How do the two isolation options differ?</b></summary>

**动态隔离** (Dynamic isolation) is an experimental Pro feature. It does not require a Windows restart and is removed when you exit the app normally. **核心隔离** (Core isolation) changes the system's CPU reservation settings and requires a restart as prompted.

Dynamic isolation does not update game rules automatically. To use isolated cores for a game, include them in the rule's core range and enable **严格核心范围** (Strict core range). Leave at least two logical cores available to the system.

</details>

<details>
<summary><b>Are settings restored when I exit?</b></summary>

Exit through the system tray menu and allow scheduling settings to be restored. Saved rules remain available for your next session.

Win32 scheduling settings persist after exit; restore them manually on the corresponding page. System core isolation must also be restored on its own page, followed by a restart as prompted.

</details>

<details>
<summary><b>Can I run it alongside LaoYing Toolkit?</b></summary>

The two apps cannot control scheduling at the same time. Exit the current app normally through the system tray before switching. FlexCore stores its own rules and settings and does not automatically import the toolkit's configuration.

</details>

## Support

**QQ community: 1109507577** (Chinese)

To report a problem, open an [issue](https://github.com/Lypc233/FlexCore/issues) with your FlexCore version, CPU model, Windows version, and steps to reproduce it. Include a screenshot if an error appears.

Downloads and release notes are available on the [Releases page](https://github.com/Lypc233/FlexCore/releases).
