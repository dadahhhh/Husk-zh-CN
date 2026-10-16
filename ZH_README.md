# Husk 2.0 简体中文构建

基于 Leviidev/Husk 的 `2.0` 标签（build 109），许可证为 GPL-2.0-or-later。
汉化词条复用了上游 PR #49 的简体中文翻译，并补充新版界面和 24 条常见问题。

应用和两个扩展由 Xcode 重新编译。QEMU、ANGLE、MoltenVK 和安卓运行资源
来自与源码版本一致的官方 2.0 IPA，下载后使用固定 SHA256 验证。
应用中的原始技术日志、第三方游戏名称、商店介绍和安卓系统内部界面不在汉化范围内。

- 原项目：https://github.com/Leviidev/Husk
- 基础版本：https://github.com/Leviidev/Husk/tree/2.0
- 翻译参考：https://github.com/Leviidev/Husk/pull/49

`src/app/Shared/HuskL10n.swift` 处理 String 类型界面文字及带参数的提示。
翻译表位于 `src/app/Husk/Resources/husk-zh-Hans.json`，系统控件使用
`zh-Hans.lproj/Localizable.strings`。FAQ 原文直接替换为中文，以便中文搜索。

IPA 采用上游的 ad-hoc 签名流程打包，普通侧载安装需由工具重新签名。
汉化不改变 JIT、配对、游戏兼容性或最低系统版本。
