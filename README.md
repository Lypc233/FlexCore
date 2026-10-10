<div align="center">

<img src="assets/flexcore.png" alt="FlexCore" width="64" height="64">

# FlexCore

面向 Windows 游戏用户的核心调度工具。

**简体中文** · [English](README.en.md)

<p>
  <img src="https://img.shields.io/badge/Windows-x64-0078D4?style=flat-square" alt="Windows x64">
  <a href="https://github.com/Lypc233/FlexCore/releases/latest"><img src="https://img.shields.io/github/v/release/Lypc233/FlexCore?style=flat-square&amp;color=E62B35&amp;label=Release" alt="最新版本"></a>
</p>

[下载最新版](https://github.com/Lypc233/FlexCore/releases/latest) · [夸克网盘](https://pan.quark.cn/s/fb393ac897ea) · [问题反馈](https://github.com/Lypc233/FlexCore/issues)

</div>

## 能做什么

FlexCore 可以为游戏和后台程序分配 CPU 核心，按进程保存调度规则，并在托盘运行时持续应用。

| 功能 | 说明 |
| :--- | :--- |
| **核心分配** | 查看进程和 CPU 核心布局，按 CCD、性能核 / 能效核选择可用核心。 |
| **游戏调度** | V1–V8 多种模式，支持优先核心与强绑；V8「双星」支持双首核调度。 |
| **后台进程管理** | 将后台程序分组，统一设置核心范围和 CPU、内存、I/O 优先级。 |
| **规则保存** | 按游戏进程保存设置，匹配后自动应用，可随时启用或停用。 |
| **核心隔离** | 提供需要重启的系统核心隔离，以及无需重启的动态核心热隔离（Pro）。 |
| **Win32 调度** | 调整前台程序调度偏好，提供预设、自定义数值和恢复入口。 |

基础调度功能免费使用。**Pro** 提供 V9「揽月」和动态核心热隔离；可在软件内查看与激活，首次激活需要联网，成功后重启软件即可使用，日常使用支持离线。

## 开始使用

1. **下载并运行**：在 [Releases](https://github.com/Lypc233/FlexCore/releases/latest) 的 **Assets** 中下载 `.exe`，运行时允许管理员权限。也可使用上方夸克网盘，无提取码。
2. **找到游戏**：启动游戏，在「核心分配 → 进程管理」里找到实际的游戏进程，确认 `.exe` 名称。
3. **设置规则**：在核心布局中选择核心，再到「调度规则」确认游戏进程和调度模式，保存规则。初次使用可先保留默认优先级，再按需要调整。
4. **开始游戏**：确认规则已启用、应用状态正常，让 FlexCore 保持运行；收进托盘后会继续调度。

调度效果会随处理器、系统和游戏变化。建议一次只调整一项，用同一场景对比帧时间和实际手感。

## 常见问题

<details>
<summary><b>动态隔离和普通核心隔离有什么区别？</b></summary>

「动态隔离」是 Pro 实验功能，无需重启系统，正常退出软件时解除；「核心隔离」修改系统核心保留设置，需要按页面提示重启。

动态隔离不会自动修改游戏规则。让游戏使用隔离核心时，还需要在「调度规则」里选中对应范围并启用「严格核心范围」。建议至少给系统留下两个逻辑核心。

</details>

<details>
<summary><b>退出软件后，设置会恢复吗？</b></summary>

请从托盘菜单正常退出，等待调度恢复完成。已保存的规则会保留，便于下次使用。

Win32 调度设置会持久保留，退出软件不会撤销，需要在对应页面手动恢复；系统核心隔离也要在对应页面恢复，并按提示重启。

</details>

<details>
<summary><b>能和老嘤超频优化工具箱一起用吗？</b></summary>

两者不能同时接管调度。切换前，先从托盘正常退出当前软件，再启动另一款。FlexCore 的规则和设置独立保存，不会自动导入工具箱配置。

</details>

## 交流与反馈

**QQ 交流群：1109507577**

遇到问题可以到 [Issues](https://github.com/Lypc233/FlexCore/issues) 留言，附上软件版本、CPU 型号、Windows 版本和复现步骤；有报错时带上截图，会更容易定位。

版本更新和下载文件见 [Releases](https://github.com/Lypc233/FlexCore/releases)。
