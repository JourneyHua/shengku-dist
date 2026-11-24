# 声库 · Shengku

声库是一款 **Windows x64 本地音乐播放器与个人音乐资料库**。你可以扫描自己的音乐目录，也可以先整理艺人、专辑、发行版次、曲目和 MV 资料，再把对应的本地音频关联到具体版次。

**[下载最新正式版](https://github.com/JourneyHua/shengku-dist/releases/latest)** · [查看所有版本](https://github.com/JourneyHua/shengku-dist/releases)

## 主要功能

- **播放和管理本地音乐**：扫描目录，按艺人、专辑和曲目浏览，使用播放队列、收藏、歌单和本地歌词。扫描和关联保留原音频文件。
- **整理发行资料**：浏览艺人档案、发行时间线和曲目资料。同一作品的不同版次可以归组，每个版次保留各自的曲目和本地音频关联。
- **核对来源与关联**：从公开来源获取目录资料，预览差异后确认。通过「待关联音频」「待关联专辑」和「独立整理」处理需要核对的记录。

## 下载和运行

1. 在最新版的 **Assets** 中下载 `Shengku-<版本>-win-x64.zip`。同名 `.sha256` 文件可用于核对下载完整性。
2. 安装 **Windows x64 的 .NET Desktop Runtime 10**。已安装的兼容桌面运行时可继续使用。
3. 完整解压 ZIP，打开 `Shengku-win-x64`，运行 `Shengku.exe`。首次使用可从「本地专辑」添加或扫描音乐目录。

[下载 .NET Desktop Runtime 10](https://dotnet.microsoft.com/zh-cn/download/dotnet/10.0)

| 使用场景 | 需要的组件 |
| --- | --- |
| 打开声库、浏览和整理资料 | .NET Desktop Runtime 10（x64） |
| 播放本地音频 | mpv |
| 按需使用部分视频功能 | yt-dlp、Deno 或 Node.js，视操作需要 FFmpeg 和 ffprobe |

轻量包不附带外部工具。可在「设置与资料来源 → 外部工具」检测已安装的工具、指定路径或按需下载。

## 更新与资料目录

- 在「设置与资料来源 → 应用更新」检查更新。应用会核对包大小和 SHA256，安装前备份上一版程序文件。
- 默认资料保存在 `%LOCALAPPDATA%\Shengku\data`。如果通过 `--data-dir` 使用自定义目录，换版本时继续指定同一目录。导出及恢复资料可从「目录与备份」进入。
- 此仓库提供正式便携包和应用更新清单 [latest.json](latest.json)。各版本的实际功能和变更以 [Releases](https://github.com/JourneyHua/shengku-dist/releases) 为准。

## 反馈问题

请附上声库版本、Windows 版本、复现步骤，以及去除个人路径和账号信息的错误提示。 [提交反馈](https://github.com/JourneyHua/shengku-dist/issues/new)
