# MC到搅拌机
Minecraft 世界/模型导出到 Blender 的工具与教程合集

## 📖 项目介绍
本项目是一套完整的流程方案，帮助你将 Minecraft 中的建筑、模型、地图世界无损导出，导入 Blender 进行渲染、动画、建模等二次创作。

## ✨ 功能特点
- 提供 Minecraft 端导出工具/脚本
- 适配 Blender 的导入插件与材质修复方案
- 附带详细图文教程与示例文件
- 解决模型发黑、贴图丢失、透明材质异常等常见问题

## 🎮 使用教程
### 1. Minecraft 端导出
1.  解压本项目提供的导出工具/模组
2.  打开文件里的应用程序
3.  进入需要导出的世界（存档的目录为英文，可以将level.dat和region文件复制放到另一个地方），等待区块加载完成
4.  使用导出指令/工具框选需要的区域，执行导出（看自身想要的）
5.  保存好导出的模型文件与贴图文件夹

### 2. Blender 端导入与修复
1.  安装项目配套的 Blender 导入插件
2.  打开 Blender，进入 编辑 (Edit) > 偏好设置 (Preferences) > 插件 (Add-ons)点击 安装 (Install)，选择你下载好的 MCprep 插件压缩包进行安装，然后将其启用
3.  新建工程，导入导出的模型文件
5.  在 MCprep 面板里，找到 Prep Materials（材质预处理）按钮，点击使用插件一键修复材质、透明贴图
6.  调整灯光与镜头，即可开始渲染创作
7.  如需其他材质，可自行下载替换

## 📁 项目结构
MC 到搅拌机 /
├── README.md               # 项目说明（你正在看的）
├── LICENSE                 # 开源协议（MIT）
├── blender-addon/          # Blender 导入插件
├── mc-export-tool/         # Minecraft 导出工具 / 模组
├── examples/               # 示例模型与工程文件
└── docs/                   # 详细图文教程

## 📥 资源下载说明

###1. 核心工具文件（直接从仓库获取）
以下文件已包含在本仓库中，可直接点击下载：
- Blender 导入插件：`/blender-addon/MC_Importer.py`
- 基础示例模型：`/examples/sample_building.obj`
- 原版基础材质：`/assets/textures/terrainExt.png`

###2. 完整资源包（推荐下载）
包含全套材质包、示例工程与扩展工具，可通过 GitHub Release 下载：
[👉 点击下载：MC到搅拌机 完整资源包 v1.0](https://github.com/shijianhuiyi/MC to Blender/releases/tag/v1.0)


### 3. 补充材质包（可选）
如需其他风格的 Minecraft 材质贴图，可自行下载后替换：
- DokuCraft 系列（写实风格）：[CurseForge 下载地址](https://www.curseforge.com/minecraft/texture-packs/dokucraft)
- JG-RTX 系列（光影追踪风格）：[PlanetMinecraft 下载地址](https://www.planetminecraft.com/texture_pack/jg-rtx/)
  
下载后，将材质包内的 `terrainExt_*.png` 文件替换 `/assets/textures/` 文件夹中的对应文件即可。

## ⚠️ 常见问题
- 模型导入后发黑：使用插件修复材质，检查贴图文件夹路径
- 树叶/玻璃不透明：开启插件的「透明材质适配」功能
- 导出时模型缺失：确保区块加载完全后再执行导出
- 注意目前blender只能显示原版的物品和物种，对于其他的材质包无法显示，需要用到blender本身带的颜色

## 📜 开源协议
本项目基于 MIT 协议开源，你可以自由使用、修改与分享，只需保留原作者的版权声明即可。
