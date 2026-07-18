# Zygisk-Il2CppDumper

[![License](https://img.shields.io/github/license/iChenAi/Zygisk-Il2CppDumper?style=flat-square)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/iChenAi/Zygisk-Il2CppDumper?style=flat-square)](https://github.com/iChenAi/Zygisk-Il2CppDumper/stargazers)

Zygisk 版 Il2CppDumper，在游戏运行时 dump il2cpp 数据，可以绕过保护、加密以及混淆。

> 基于 [Perfare/Zygisk-Il2CppDumper](https://github.com/Perfare/Zygisk-Il2CppDumper) 修改，适配新版 GitHub Actions。

---

## ✨ 特性

- 🔓 运行时 dump，绕过 il2cpp 保护
- 🛡 支持加密和混淆的 il2cpp 数据
- 🤖 支持 GitHub Actions 自动构建
- 📦 生成的模块可直接在 Magisk 中安装
- 🔧 支持 Android Studio 本地编译

## 📋 使用方法

### 方法一：GitHub Actions（推荐）

1. **Fork** 本项目
2. 在你 fork 的项目中选择 **Actions** 选项卡
3. 在左侧边栏中，点击 **Build**
4. 选择 **Run workflow**
5. 输入游戏包名并点击 **Run workflow**
6. 等待操作完成并下载产物

### 方法二：Android Studio 本地编译

1. 下载源码
2. 编辑 `game.h`，修改 `GamePackageName` 为游戏包名
3. 使用 Android Studio 运行 gradle 任务 `:module:assembleRelease`
4. 编译产物在 `out` 文件夹下

## 🚀 安装

1. 安装 [Magisk](https://github.com/topjohnwu/Magisk) v24 以上版本并开启 Zygisk
2. 在 Magisk 中安装生成的模块
3. 启动游戏，会在 `/data/data/<GamePackageName>/files/` 目录下生成 `dump.cs`

## 📄 License

GPL-3.0 — 详见 [LICENSE](LICENSE)。

---

<p align="center">
  <sub>Made with ❤️ by <a href="https://github.com/iChenAi">ChenAi</a></sub>
</p>