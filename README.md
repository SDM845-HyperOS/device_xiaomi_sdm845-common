# Common device tree for Xiaomi SDM845 based devices

Copyright (C) 2025 - The AOSP Project

## 项目概述

这是小米SDM845芯片组设备的通用设备树项目，属于HyperOS项目的一部分。该项目为基于高通SDM845平台的小米设备提供了统一的硬件抽象层和系统配置，支持多个设备型号的共用配置。

## 支持的设备

基于SDM845的小米设备，包括但不限于：
- 小米8系列
- 小米MIX 2S
- POCO F1
- 其他基于SDM845的小米设备

## 项目结构

```
├── Android.bp                    # Soong构建系统配置
├── sdm845.mk                    # 主要产品配置文件
├── BoardConfigCommon.mk         # 板级配置文件
├── manifest.xml                 # HIDL接口清单
├── framework_compatibility_matrix.xml  # 兼容性矩阵
├── proprietary-files.txt        # 专有文件列表
├── audio/                       # 音频子系统配置
├── wifi/                        # WiFi配置
├── init/                        # 初始化脚本
├── sepolicy/                    # SELinux安全策略
├── overlay/                     # 资源覆盖层
├── power/                       # 电源管理
├── recovery/                    # 恢复模式配置
├── parts/                       # 小米定制组件
├── udfps/                       # 屏下指纹配置
├── keylayout/                   # 键位布局配置
├── *.prop                       # 系统属性配置文件
└── releasetools.py             # 发布工具脚本
```

## 贡献指南

### 代码规范
- 遵循Android开源项目代码规范
- 提交前确保代码通过lint检查
- 添加适当的注释和文档

### 提交流程
1. Fork项目到个人仓库
2. 创建功能分支进行开发
3. 提交Pull Request并描述改动
4. 等待代码审查和合并

## 许可证

本项目采用Apache 2.0许可证开源，详见[LICENSE](LICENSE)文件。

## 致谢

- **AOSP**：Android开源项目
- **Qualcomm**：SDM845平台技术支持
- **LineageOS**：社区框架和接口支持
- **HyperOS Project**：项目维护和社区支持

## 反馈与支持

如有问题或建议，请通过以下方式联系：
- 提交GitHub Issue
- 加入开发者社区讨论
- 邮件联系项目维护者

---

**注意**：本设备树仅适用于小米SDM845设备，使用前请确认您的设备型号。编译和刷机有风险，请确保了解相关风险并做好数据备份。
