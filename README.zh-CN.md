# JsonlLens — 面向 10GB+ JSONL、NDJSON 和 Parquet 文件的高速 Windows 查看器

**语言：** [English](README.md) · [日本語](README.ja.md) · 简体中文

<p align="center">
  <a href="https://apps.microsoft.com/detail/9N9X7K90R64G">
    <img src="https://get.microsoft.com/images/en-us%20dark.svg" width="260" alt="从 Microsoft Store 获取" />
  </a>
</p>

<p align="center"><strong>在 Windows 上快速打开、搜索、检查和查询多 GB 数据文件，避免传统文本编辑器卡顿。</strong></p>

![真实运行中的 JsonlLens Windows 应用](assets/jsonllens-demo.gif)

上方 GIF 来自实际运行的 JsonlLens Windows 桌面版本。JsonlLens 通过稀疏索引、虚拟化行显示和 DuckDB 流式查询，让工程师能够处理传统编辑器难以打开的大型数据文件。

## 主要功能

- 快速显示大型 JSONL / NDJSON 文件的第一页
- 分页查看文件，不把完整数据加载进界面
- 自动推断字段，并显示为可排序列
- 快速筛选与 DuckDB SQL 控制台
- JSON 详情检查器和原始行视图
- 只读设计，避免误修改生产导出和日志
- 支持 English、简体中文和日本語三种界面语言，可在应用菜单中切换
- 支持 `.jsonl`、`.ndjson`、`.parquet`、`.csv` 和结构化日志

## 性能基准快照

以下数据来自 Windows 11 x64、SSD、未安装编辑器扩展时打开 5 GB 合成 JSONL 文件的代表性测试。磁盘速度、杀毒软件、扩展和文件结构都会影响结果，建议按相同流程在自己的设备上复测。

| 查看器 | 首次可操作视图 | 峰值工作集内存 | 结果 |
| --- | ---: | ---: | --- |
| **JsonlLens** | **0.84 秒** | **183 MB** | 可交互分页和筛选 |
| VS Code（5 GB JSONL） | 2 分 41 秒 | 2.78 GB | 加载期间出现无响应 |

## 从 Microsoft Store 获取

通过 Microsoft Store 安装签名版 Windows 软件包，并使用系统的 Store 更新流程。

<p align="center">
  <a href="https://apps.microsoft.com/detail/9N9X7K90R64G">
    <img src="https://get.microsoft.com/images/en-us%20dark.svg" width="260" alt="从 Microsoft Store 获取" />
  </a>
</p>

- Windows 10 / 11，x64
- 面向大型数据文件的只读查看器
- Pro 版本提供 SQL 和导出能力

## 反馈

提交 Issue 时，请附上 Windows 版本、文件格式和复现步骤。分享样例或截图前，请删除密钥、个人信息和其他敏感数据。

