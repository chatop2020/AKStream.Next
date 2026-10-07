# AKStream.Next

**把视频接入、实时观看、录像检索和音视频协作连接到业务系统。**

**Connect video sources, live viewing, recording search, and real-time collaboration to your business applications.**

[官网 / Website](https://softnvr.com/) · [下载 / Releases](https://github.com/chatop2020/AKStream.Next/releases) · [中文文档](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN) · [English documentation](https://github.com/chatop2020/AKStream.Next/wiki/en-US) · [AI integration Skill](https://github.com/chatop2020/AKStream.Next/wiki/Integration-Skill)

## 中文介绍

AKStream.Next 是面向视频监控、流媒体接入和实时音视频场景的视频管理平台。它围绕设备、通道、录像、媒体节点和会议，提供统一的操作入口，让摄像机接入、实时预览、录像回放、智能检索、协议互通、运维管理和第三方业务集成形成完整工作流程。

你可以先从一台服务器、一台摄像机开始，完成安装、首次配置和首路视频；也可以根据业务规模规划多个节点，并通过公开 API、事件通知和 RTC SDK 将视频能力接入自己的应用。

### 适合哪些场景

- **园区、楼宇与企业监控**：集中接入设备，统一预览、录像、回放、云台控制和视频墙。
- **多品牌设备与平台互通**：按现场条件选择 GB28181、ONVIF 或 RTSP，处理设备接入与上级平台级联。
- **录像查找与事后复核**：通过时间、通道、文字描述或参考图片缩小范围，定位原录像中的命中片段。
- **业务系统与行业应用**：为管理平台、告警系统、调度系统或移动应用提供视频播放、录像和会议能力。
- **远程协作与音视频会议**：使用 RTC 房间、成员管理、屏幕共享和会议录制，让人员音视频参与业务流程。
- **需要掌握数据与部署环境的项目**：在自己的服务器或容器环境部署，规划录像、模型、索引和计算资源。

### 产品优势

| 优势 | 对使用者的价值 |
| --- | --- |
| 视频业务统一管理 | 用设备、通道和录像的统一视图完成接入、观看、控制和回放，减少在多个工具间切换。 |
| 兼顾设备接入与业务集成 | 摄像机/NVR 接入、平台级联、公开 API 和事件通知可以配合使用，视频不止停留在预览页面。 |
| 把录像结果连接到原始画面 | 智能搜索结果包含通道、原录像和命中时间，便于跳转播放并复核结果。 |
| 本地部署与本地图文检索 | 可在本地节点处理录像与配套模型，不要求把视频画面发送到外部模型服务。 |
| 逐步扩展的部署方式 | 支持单机部署与多节点规划，按节点、媒体、数据库、存储和网络需求安排资源。 |
| 运行状态与配置可核对 | 提供节点状态、参数差异、配置生效情况、任务、日志和告警入口，便于发现问题并确认操作结果。 |
| 公开接口与完整对接指引 | 中英文指南、公开接口契约、Postman 资料和 AI Skill 帮助集成方从实际用例开始对接。 |
| 按系统与架构交付 | Windows、Linux、macOS 和 Docker 均有对应发布目标，便于选择与现有环境匹配的包。 |

### 功能全景

| 模块 | 主要能力 | 文档入口 |
| --- | --- | --- |
| 设备与通道 | 摄像机、NVR、下级平台及视频地址接入；设备发现、通道同步、分组、状态查看、启停与删除。 | [设备接入](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--devices--home) |
| ONVIF | 设备发现、能力与视频 Profile 获取，以及设备支持范围内的图像参数、云台和事件功能。 | [ONVIF 指南](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--devices--onvif) |
| GB28181 | 设备注册与保活、目录和通道管理、直播与回放、云台/预置位、对讲及平台级联；具体能力需结合设备支持核对。 | [GB28181 指南](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--devices--gb28181) |
| RTSP 与流媒体播放 | 按地址接入视频，查看流状态并选择适合浏览器与网络的播放方式。 | [RTSP 接入](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--devices--rtsp)、[实时观看](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--video--live) |
| 设备控制 | 云台方向、缩放、预置位、图像参数与语音对讲；按协议及设备能力提供操作。 | [设备控制](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--devices--control) |
| 录像与存储 | 自动/手工录像、录像计划、存储目录、录像查询、回放、下载、裁剪和文件管理。 | [录像](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--video--recording)、[回放与裁剪](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--video--playback) |
| AI 录像智能检索 | 输入文字或参考图片，按通道、时间、相似度和结果数量查找已索引内容，查看缩略图并跳到命中时刻播放。 | [图文搜视频](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--video--intelligent-search) |
| 截图与视频墙 | 周期截图查询与下载、独立视频墙、节目编排和多路画面展示。 | [周期截图](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--video--snapshots)、[视频墙](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--video--display-wall) |
| RTC 音视频协作 | 会议/房间、成员与媒体管理、摄像头/麦克风、屏幕共享、聊天/白板和会议录制与回放；终端兼容性按对应 SDK 与设备验收。 | [RTC 使用](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--video--rtc)、[录制与回放](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--sdk--recording) |
| RTC SDK 集成 | Web/H5/WebView、Android、iOS、UniApp 与 uni-app x 的接入指南、身份与入会流程、函数参考和逐端验收。 | [SDK 文档](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--sdk--home) |
| API 与业务对接 | 设备、通道、播放、录像、截图、RTC、账号权限及系统运维等公开接口，配套认证、权限、请求模型与错误处理说明。 | [API 起步](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--development--home)、[API 目录](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--development--api-index) |
| Webhook 与事件联动 | 配置独立接收方案、选择事件范围、测试投递，并查看重试与投递记录，连接外部业务系统。 | [Webhook](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--operations--outbound-webhook) |
| 安全与权限 | 首次管理员初始化、登录与账号管理、角色和权限、API 身份、播放访问控制及安全配置。 | [安全设置](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--operations--security)、[API 安全](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--development--api-security) |
| 系统与运维 | 节点状态、配置调整、任务、日志、告警、备份恢复、升级回滚和故障定位。 | [系统管理](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--modules--platform)、[运维指南](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--operations--home) |
| 授权与离线文档 | 功能授权、离线授权申请与导入、版本下载校验，以及与在线 Wiki 同源的包内文档和 AI 对接 Skill。 | [授权说明](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--licensing--home)、[Skill 目录](https://github.com/chatop2020/AKStream.Next/wiki/Integration-Skill) |

### 部署与集成

| 环境 | 发布目标 | 安装指南 |
| --- | --- | --- |
| Linux | x64 / ARM64 | [Linux 安装](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--deployment--linux) |
| Windows | x64 / ARM64 | [Windows 安装](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--deployment--windows) |
| macOS | Intel x64 / Apple Silicon ARM64 | [macOS 安装](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--deployment--macos) |
| Docker | Linux AMD64 / ARM64 离线镜像包 | [Docker 安装](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--deployment--docker) |

部署前按通道数量、录像保存周期、存储容量、并发播放、RTC 带宽和检索预算规划资源。对外提供服务时同时规划端口、域名、HTTPS、NAT、STUN/TURN 以及持久化数据目录。安装后可以使用 `akn` 管理服务、状态、日志和升级，具体命令以对应平台指南为准。

集成方可以先通过公开 API 跑通一条视频播放或录像调用链，再接入事件通知与 RTC。AI 对接 Skill 提供使用说明、接口目录、公开契约、接入示例和专题指南；在 [Skill 页面](https://github.com/chatop2020/AKStream.Next/wiki/Integration-Skill) 中可按目录阅读，发布包中的文档也提供可安装的 Skill 目录。

### 从安装包到第一路画面

1. 在 [官网](https://softnvr.com/) 了解适用场景、使用条件和功能授权。
2. 阅读 [部署规划](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--deployment--plan) 和 [安装方式](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--deployment--install)，选择系统与架构。
3. 从 [Releases](https://github.com/chatop2020/AKStream.Next/releases) 下载包，核对 SHA-256 并完整解压。
4. 完成 [首次配置](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--deployment--first-run)，登录后 [接入第一路视频](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--start--first-value)。
5. 确认实时观看、录像生成和回放正常，再逐步开启视频墙、检索、级联或 RTC。
6. 出现问题时按 [可见现象排查](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--operations--problem-finder)，集成程序则从 [API 起步](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--development--home) 开始。

### 版本、模型与兼容性

安装包的平台、架构和组件以对应 Release 为准。高级功能需要匹配的授权、模型、硬件后端及网络配置；模型权重独立分发，不随本公开安装包提供。智能检索只覆盖实际完成索引并仍可读取的录像，相似度不是识别概率。RTC、设备控制和协议互通也需要在目标终端、设备和网络中验收。

详细边界请查阅 [兼容性说明](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--reference--compatibility)、[检索模型与硬件选型](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--video--recording-search-models) 和 [RTC 验收](https://github.com/chatop2020/AKStream.Next/wiki/zh-CN--sdk--acceptance)。反馈问题时请说明版本、系统/架构、相关设备或网络条件、操作步骤和已脱敏日志。

本仓库提供官方发布包和公开产品文档。软件使用、功能授权和支持条件请参阅官网；公开仓库访问不授予产品源码或其他资产的使用权。

## English introduction

AKStream.Next is a video management platform for surveillance, streaming integration, and real-time audio and video. It provides a unified workflow around devices, channels, recordings, media nodes, and meetings: connect video sources, watch live feeds, manage recordings, search indexed footage, interoperate with protocols, operate the system, and integrate business applications.

Start with one server and one camera, complete setup, and verify the first video. For larger deployments, plan multiple nodes and use public APIs, event notifications, and RTC SDKs to add video capabilities to your own applications.

### Typical use cases

- **Enterprise, building, and campus surveillance**: centralized device access, live preview, recording, playback, PTZ control, and video walls.
- **Multi-vendor device and platform integration**: choose GB28181, ONVIF, or RTSP according to the site and connect upstream platforms where supported.
- **Recording search and incident review**: narrow footage by time, channel, text description, or reference image and jump to the matching moment in the original recording.
- **Business and industry applications**: add video playback, recording, and meetings to management, alarm, dispatch, and mobile applications.
- **Remote audio/video collaboration**: use RTC rooms, participant management, screen sharing, and meeting recording in business workflows.
- **Projects that control their own deployment and data**: run on your servers or containers and plan storage, models, indexes, and compute resources.

### Product strengths

| Strength | Practical value |
| --- | --- |
| Unified video operations | Manage access, viewing, control, and playback through consistent device, channel, and recording views. |
| Device access and business integration together | Combine camera/NVR access, platform cascading, APIs, and event notifications instead of stopping at a preview screen. |
| Search results connected to original footage | Results identify the channel, recording, and timestamp so users can play and review the match. |
| Local deployment and local image/text search | Process recordings and the matching models on local nodes without requiring footage to be sent to an external model service. |
| Deployment that can grow incrementally | Plan a single machine or multiple nodes around media, database, storage, and network needs. |
| Visible operating and configuration state | Inspect nodes, parameter differences, effective settings, tasks, logs, and alerts when verifying changes or diagnosing failures. |
| Public contracts and integration guidance | Bilingual guides, API contracts, Postman resources, and an AI Skill help integrators begin with concrete use cases. |
| Packages for the target environment | Choose Windows, Linux, macOS, or Docker packages matching the operating system and architecture. |

### Feature overview

| Area | Main capabilities | Documentation |
| --- | --- | --- |
| Devices and channels | Camera, NVR, downstream platform, and video-URL integration; discovery, channel synchronization, grouping, state, start/stop, and deletion. | [Device integration](https://github.com/chatop2020/AKStream.Next/wiki/en-US--devices--home) |
| ONVIF | Discovery, device capabilities, video Profiles, and supported imaging, PTZ, and event operations. | [ONVIF](https://github.com/chatop2020/AKStream.Next/wiki/en-US--devices--onvif) |
| GB28181 | Registration, keepalive, catalogs and channels, live viewing and playback, PTZ/presets, talkback, and cascading; verify the device's supported capabilities. | [GB28181](https://github.com/chatop2020/AKStream.Next/wiki/en-US--devices--gb28181) |
| RTSP and streaming playback | Connect video URLs, inspect stream state, and select a playback method suitable for the browser and network. | [RTSP](https://github.com/chatop2020/AKStream.Next/wiki/en-US--devices--rtsp), [Live viewing](https://github.com/chatop2020/AKStream.Next/wiki/en-US--video--live) |
| Device control | PTZ movement and zoom, presets, imaging parameters, and talkback according to protocol and device support. | [Device control](https://github.com/chatop2020/AKStream.Next/wiki/en-US--devices--control) |
| Recording and storage | Manual and scheduled recording, storage locations, search, playback, download, clipping, and file management. | [Recording](https://github.com/chatop2020/AKStream.Next/wiki/en-US--video--recording), [Playback](https://github.com/chatop2020/AKStream.Next/wiki/en-US--video--playback) |
| AI recording search | Search indexed content with text or a reference image; filter by channel, time, similarity, and result count, then view thumbnails and play the matching moment. | [Image/text search](https://github.com/chatop2020/AKStream.Next/wiki/en-US--video--intelligent-search) |
| Snapshots and video walls | Periodic snapshot retrieval and download, independent video walls, program scheduling, and multiple video views. | [Snapshots](https://github.com/chatop2020/AKStream.Next/wiki/en-US--video--snapshots), [Video walls](https://github.com/chatop2020/AKStream.Next/wiki/en-US--video--display-wall) |
| RTC collaboration | Rooms/meetings, participants and media, cameras and microphones, screen sharing, chat/whiteboards, meeting recording, and playback; validate each target SDK and device. | [RTC](https://github.com/chatop2020/AKStream.Next/wiki/en-US--video--rtc), [Meeting recording](https://github.com/chatop2020/AKStream.Next/wiki/en-US--sdk--recording) |
| RTC SDK integration | Web/H5/WebView, Android, iOS, UniApp, and uni-app x guides; identity and joining flows, function references, and per-client acceptance. | [SDK guides](https://github.com/chatop2020/AKStream.Next/wiki/en-US--sdk--home) |
| APIs and business integration | Public device, channel, playback, recording, snapshot, RTC, account/permission, and operations APIs, with authentication, request models, and error handling. | [Start integrating](https://github.com/chatop2020/AKStream.Next/wiki/en-US--development--home), [API index](https://github.com/chatop2020/AKStream.Next/wiki/en-US--development--api-index) |
| Webhooks and events | Independent receivers, event selection, test delivery, retries, and delivery records for external applications. | [Webhooks](https://github.com/chatop2020/AKStream.Next/wiki/en-US--operations--outbound-webhook) |
| Security and permissions | Initial administrator setup, authentication and account management, roles and permissions, API identity, playback access, and security settings. | [Security](https://github.com/chatop2020/AKStream.Next/wiki/en-US--operations--security), [API security](https://github.com/chatop2020/AKStream.Next/wiki/en-US--development--api-security) |
| Operations | Node status, configuration changes, tasks, logs, alerts, backup/restore, upgrades/rollback, and troubleshooting. | [System management](https://github.com/chatop2020/AKStream.Next/wiki/en-US--modules--platform), [Operations](https://github.com/chatop2020/AKStream.Next/wiki/en-US--operations--home) |
| Licensing and offline documentation | Feature licensing, offline license requests/import, release verification, and package documentation plus the AI Skill from the same public source as the Wiki. | [Licensing](https://github.com/chatop2020/AKStream.Next/wiki/en-US--licensing--home), [Skill directory](https://github.com/chatop2020/AKStream.Next/wiki/Integration-Skill) |

### Deployment and integration

| Environment | Release targets | Installation |
| --- | --- | --- |
| Linux | x64 / ARM64 | [Linux guide](https://github.com/chatop2020/AKStream.Next/wiki/en-US--deployment--linux) |
| Windows | x64 / ARM64 | [Windows guide](https://github.com/chatop2020/AKStream.Next/wiki/en-US--deployment--windows) |
| macOS | Intel x64 / Apple Silicon ARM64 | [macOS guide](https://github.com/chatop2020/AKStream.Next/wiki/en-US--deployment--macos) |
| Docker | Linux AMD64 / ARM64 offline image packages | [Docker guide](https://github.com/chatop2020/AKStream.Next/wiki/en-US--deployment--docker) |

Plan capacity around channels, retention, storage, simultaneous viewing, RTC bandwidth, and search budgets. For external access, plan ports, domains, HTTPS, NAT, STUN/TURN, and persistent data directories. Use the platform-specific `akn` guides to manage services, state, logs, and upgrades after installation.

Integrators can first complete one playback or recording API flow and then add events and RTC. The AI integration Skill includes usage instructions, an API index, public contracts, recipes, and topic guides. Browse its [directory](https://github.com/chatop2020/AKStream.Next/wiki/Integration-Skill), or install the Skill supplied with the release documentation.

### From the package to the first video

1. Visit the [website](https://softnvr.com/) for use cases, terms of use, and feature licensing.
2. Read [deployment planning](https://github.com/chatop2020/AKStream.Next/wiki/en-US--deployment--plan) and [installation choices](https://github.com/chatop2020/AKStream.Next/wiki/en-US--deployment--install), then select the system and architecture.
3. Download from [Releases](https://github.com/chatop2020/AKStream.Next/releases), verify SHA-256, and extract the complete package.
4. Complete [initial setup](https://github.com/chatop2020/AKStream.Next/wiki/en-US--deployment--first-run) and [connect the first video](https://github.com/chatop2020/AKStream.Next/wiki/en-US--start--first-value).
5. Verify live viewing, recording, and playback before adding video walls, search, cascading, or RTC.
6. Troubleshoot by [visible symptom](https://github.com/chatop2020/AKStream.Next/wiki/en-US--operations--problem-finder); start application integration with the [API guide](https://github.com/chatop2020/AKStream.Next/wiki/en-US--development--home).

### Versions, models, and compatibility

Package platforms, architectures, and included components are defined by each Release. Advanced features need the appropriate license, models, hardware backend, and network configuration. Model weights are distributed separately and are not included in these public installation packages. Intelligent search covers footage that has actually been indexed and remains readable; similarity is not a recognition probability. Validate RTC, device control, and protocol interoperability with the target clients, equipment, and network.

See [compatibility](https://github.com/chatop2020/AKStream.Next/wiki/en-US--reference--compatibility), [search models and hardware](https://github.com/chatop2020/AKStream.Next/wiki/en-US--video--recording-search-models), and [RTC acceptance](https://github.com/chatop2020/AKStream.Next/wiki/en-US--sdk--acceptance). When reporting an issue, include the version, system/architecture, device or network conditions, reproduction steps, and sanitized logs.

This repository distributes official packages and public product documentation. Refer to the website for software use, feature licensing, and support terms. Public repository access does not grant rights to the product source code or other assets.

<!-- documentation-version: 1.0.0.169; wiki-commit: 239e6d2e3e4dc08d2261a4be878aab4301860b5c -->
