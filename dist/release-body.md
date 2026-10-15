# EmuBox v1.1.0 — 首个官方正式稳定版

> 从 EmuHub-CN 独立更名而来的安卓端游戏模拟器聚合管理工具箱。
> 包名 `com.emubox.app` · 正式签名（CN=EmuBox）· CI 全绿 · versionCode 17

## ✨ 本版新增

- **游戏支持评估（核心）**：驱动实测成功后，按实测 GPU 厂商推导驱动类型（Adreno→Turnip / Mali→PanVK / 系统），对 Windows 游戏按 D3D8/9、D3D10/11、D3D12 及 Switch 游戏（Eden/Citron）给出**支持等级分级**——基本能跑 / 可能能跑（注明缺项）/ 跑不了，独立于跑分结果展示（跑分失败也能看到评估）。
- **来源切换作者头像**：驱动专区 / 组件专区切换来源弹窗中，每个仓库条目显示 GitHub 作者头像，一眼区分来源。
- **配置推荐自动刷新**：聚合 bannerlator-game-configs 与 Winlator-Mali 社区配置，按 GPU 热度排行自动每日刷新（53 Adreno + 23 Mali 组）。

## 🔧 修复与清理

- **驱动注册表 schema 修复**：新条目 `companion` 字段数组化（此前为字符串导致 CI 校验必红），48 条全部通过校验。
- **驱动工具区彻底移除**：删除 PanProbe/PanPlay/VkTest 参考工具区及其状态残留（不再误导）。
- **运行库区精简**：移除多余的作者头像图标。
- **About 更名**：清除应用内 EmuHub 残留文案，明确 EmuBox 独立更名并保留 MIT 上游致谢。

## 🧭 核心能力

- **驱动专区**：聚合 48 个驱动源仓库（Turnip / PanVK / Qualcomm / 厂商系统），按设备 GPU 自动匹配推荐。
- **组件专区**：DXVK / VKD3D / Box64 / FEXCore 等运行库组件一键下载，多来源切换。
- **设备检测**：AdrenoTools 内置实测——实例/设备扩展、API 版本、驱动兼容判断、带宽跑分。
- **模拟器聚合**：Winlator / Eden / Citron / GameHub / Sumi 等官方源 + 每夜版（eden-ci/nightly）聚合，趋势榜与更新动态。
- **运行库专区**：VC++/.NET/解码器/字体等运行库一键下载。
- **下载管理**：断点续传、多线程、自定义目录、分类子文件夹。
- **镜像加速**：多节点带宽测速自动择优（MirrorHub）。

## 📥 安装

直接安装 APK（需允许"安装未知来源应用"）。驱动检测需已安装对应模拟器环境（Winlator/Eden）。

## 📄 许可

MIT（上游 Rodrig02005 项目致谢保留）。
