[English](README.md) · **中文** · [日本語](README.ja.md) · [한국어](README.ko.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)

> **ScsSubst 不是 ScsDriver。** ScsDriver 是 ScsDrive（https://drive.scsoi.com）的旧名，指的是把 WebDAV/NAS 挂载成本地盘的那一款，与 ScsSubst 是两个不同的软件。ScsSubst 把电脑上已存在的文件夹映射成盘符。官网：<https://subst.scsoi.com>
<p align="center">
  <img src="docs/banner.svg" alt="ScsSubst" width="100%">
</p>

<h1 align="center">ScsSubst</h1>

<p align="center">
  <strong>把文件夹变成盘符</strong><br>
  给深层目录一个盘符入口，不复制文件，像本地硬盘一样打开。<br>
  官网：<a href="https://subst.scsoi.com">https://subst.scsoi.com</a>
</p>

<p align="center">
  <a href="https://subst.scsoi.com"><img src="https://img.shields.io/badge/Website-subst.scsoi.com-0F766E?style=flat-square" alt="Website"></a>
  <a href="https://github.com/shuyingegit/scssubst/releases/latest"><img src="https://img.shields.io/github/v/release/shuyingegit/scssubst?style=flat-square&label=Release" alt="Release"></a>
  <a href="https://subst.scsoi.com/#download"><img src="https://img.shields.io/badge/Windows-10%20%2F%2011-0078D4?style=flat-square&logo=windows&logoColor=white" alt="Windows"></a>
  <a href="mailto:support@scsoi.com"><img src="https://img.shields.io/badge/Support-support%40scsoi.com-6B7280?style=flat-square" alt="Support"></a>
</p>

<p align="center">
  <a href="https://subst.scsoi.com/#download"><strong>下载</strong></a> ·
  <a href="https://subst.scsoi.com/#pricing"><strong>定价</strong></a> ·
  <a href="https://subst.scsoi.com/faq"><strong>常见问题</strong></a> ·
  <a href="https://subst.scsoi.com/compare/visual-subst-alternative"><strong>对比 Visual Subst</strong></a> ·
  <a href="https://subst.scsoi.com/guide/subst-drive-letter"><strong>使用指南</strong></a> ·
  <a href="https://github.com/shuyingegit/scssubst/releases"><strong>发行版</strong></a> ·
  <a href="https://drive.scsoi.com"><strong>ScsDrive</strong></a> ·
  <a href="https://expand.scsoi.com"><strong>ScsExpand</strong></a>
</p>

---

## 为什么选择 ScsSubst？

给深层目录一个盘符入口，不复制文件，像本地硬盘一样打开。

跑会写盘、会删文件的工具时，最怕越界乱删？给它单独一张工作盘，出不去。

<p align="center">
  <img src="docs/hero.png" alt="ScsSubst hero" width="920">
</p>

## 能用来做什么

- 常用文件夹 → 盘符
- 把工具困在一张盘里，不能越界
- 超长项目路径缩成一字母
- 多工作区，各挂各的盘

### 重点：更安全的沙箱工作盘

**给它一张出不去的工作盘**

跑会写盘、会删文件的工具时，最怕越权乱删。单独建工作目录，映射成盘符，再让工具只在这个盘里干活。

1. 建专用工作目录
2. 映射成盘符（如 Z:）
3. 把工具工作区指到 Z:

> 前提：工具工作区设在该盘下。盘符边界的实用隔离，不是内核沙箱。

<p align="center">
  <img src="docs/sandbox-usecase.png" alt="ScsSubst sandbox use case" width="920">
</p>

## 核心功能

简单、稳定、不折腾。

- **一键挂载** — 选择文件夹与盘符，一点「连接」即可映射；开启「开机自启」后，下次开机盘符自动恢复。
- **本地体验** — 在资源管理器里像普通盘符一样使用，路径更短更好记。
- **开机自启** — 可让 ScsSubst 随 Windows 启动并重新挂载已保存的映射项，下次登录后盘符即恢复。
- **轻量稳定** — 纯系统 API，不捆绑第三方文件系统驱动，绿色包体积小。
- **多映射** — 可添加多条映射，各自独立盘符，互不干扰。
- **高级选项** — 可选「管理员程序可见」、回收站等高级选项，默认保持简单。
- **安装即试用** — 默认 7 天试用；到期后用授权码激活（月 / 年 / 终身）。
- **沙箱工作盘** — 会写盘的工具常越界乱删。给它单独工作目录并映射成盘符，工作区指到该盘——越界也出不了这张盘。

## ScsSubst 不做什么

- **它不能挂网络盘。** ScsSubst 只把**本机已经存在的文件夹**映射成盘符，不支持挂载 NAS、映射的共享目录或云存储——那是 ScsDrive 的事：https://drive.scsoi.com/
- **它不是 ScsDrive。** 两者方向相反：ScsDrive 把**远程**存储挂成真实本地盘，ScsSubst 把**本地**文件夹映射成盘符。
- **它不是复制或同步工具。** 不会复制任何文件。ScsSubst 创建的是指向原文件夹的映射，不额外占用磁盘空间，读写速度与该文件夹所在磁盘一致。
- **它不是操作系统级沙箱。** 这种隔离是基于盘符边界的实用隔离：前提是把工具的工作区设为那个盘符。它本身也不会突破 Windows 的 MAX_PATH 限制。

## ScsSubst 与 subst.exe、Visual Subst、psubst、mklink /J 的区别

下表信息依据各工具的公开文档与各家官网当前公开信息整理，具体以各家官网当前公开信息为准。每款工具在各自的场景里都是合理选择，差别主要在功能范围。

| 工具 | 它是什么 | 给盘符吗？ | 注销 / 重启之后 | 适合什么场景 |
|---|---|---|---|---|
| **Windows `subst.exe`** | Windows 内置的命令行工具，为本地文件夹创建盘符映射 | 给 | 不给——映射是会话级的，注销或重启即失效；要常驻得自己写启动脚本 | 其它工具的底层机制；临时映射一次，用它最快 |
| **Visual Subst** | `subst.exe` 的免费图形前端，映射清单保存在 ini 文件里 | 给 | 保留——可在开机时按 ini 文件重建映射 | 开机自动把文件夹映射成盘符。功能面比 ScsSubst 窄，ScsSubst 的侧重点是多个映射管理、随应用启动重挂载与工作区隔离 |
| **psubst** | 用于创建盘符映射的命令行工具 | 给 | 加 `/P` 参数即可持久化 | 脚本与批处理流程，没有图形界面 |
| **vSubst** | 极小的盘符映射图形前端 | 给 | 见该工具自己的文档 | 只想点一下就完成映射的轻量界面 |
| **`mklink /J`** | Windows 内置的目录联接：目标以普通文件夹形式出现在上级路径下 | 不给——联接不会产生盘符 | 联接本身会一直有效，只要目标文件夹还在 | 兼容性最好、回收站行为正常，但很多要求盘符的教程和工具用不了 |
| **New-PSDrive** | PowerShell 的 PSDrive cmdlet | 给，但只在 PowerShell 里有效 | 不保留——PSDrive 只存在于创建它的那个 PowerShell 会话中 | 只在 PowerShell 里跑的工作流；资源管理器里看不到 |
| **ScsSubst** | Windows 工具，把本地已有文件夹映射成盘符，带映射清单，并提供提权程序与回收站相关选项 | 给 | 已保存的映射可在应用启动时重新挂载（随应用启动重挂载） | 定位：多个映射管理 + 随应用启动重挂载 + 工作区隔离。仅 Windows 10 / 11（64 位），只映射本地文件夹 |

**怎么选**

- 临时给一个文件夹要个盘符：内置的 `subst.exe` 就够了。
- 想要图形界面、开机自动重建同样的映射：Visual Subst 用 ini 文件就能做到；ScsSubst 开启「开机自启」后同样可以。
- 映射要写进脚本，包括用 `/P` 持久化：psubst 更贴合批处理流程。
- 希望目标在项目目录树里仍是一个普通文件夹、且回收站行为正常：`mklink /J` 是兼容性最好的选择，但它不给盘符。
- 需要「一个工作区一个盘符」、同时管多个文件夹、并且映射要随应用启动回来：这就是 ScsSubst。

完整对照说明：**[ScsSubst 与 Visual Subst 等方案的对比](https://subst.scsoi.com/compare/visual-subst-alternative)**。

## 下载

最新安装包: **[GitHub 发行版](https://github.com/shuyingegit/scssubst/releases/latest)** · [官网](https://subst.scsoi.com/#download)

| 包类型 | 适用场景 |
|--------|----------|
| **Portable (`.zip`)** | 解压即用（推荐） |
| **Installer (`.exe`)** | 安装程序 |

系统要求：Windows 10 / 11（64 位）

## 定价

免费试用从 7 天开始。邀请好友一起试用，双方都可以再延长。

所有套餐（含免费试用）均含技术支持：使用中遇到任何异常、报错或问题，发邮件给我们，我们会跟进排查、修复并持续改进。

价格与当前套餐见官网：https://subst.scsoi.com/

## 官网与指南

- 首页：https://subst.scsoi.com/
- 常见问题：https://subst.scsoi.com/faq
- 对比 —— ScsSubst 与 Visual Subst、`subst.exe`、`mklink /J`：https://subst.scsoi.com/compare/visual-subst-alternative
- 指南 —— subst 盘符实操步骤：https://subst.scsoi.com/guide/subst-drive-letter

## 姊妹产品

- **[ScsDrive](https://github.com/shuyingegit/scsdriver)** — 仓库标识仍是 `scsdriver`，同一产品 — [drive.scsoi.com](https://drive.scsoi.com) — 把 WebDAV / 网盘挂成 Windows 本地磁盘，像本地硬盘一样打开云端文件。
- **[ScsExpand](https://github.com/shuyingegit/scsexpand)** — [expand.scsoi.com](https://expand.scsoi.com) — 把同一块物理磁盘上的空闲空间划给 C 盘，文件原地保留。

更多 SCSOI 产品 —— [公司官网](https://scsoi.com)

## 常见问题

**ScsSubst 和 Windows 自带的 `subst.exe` 是什么关系？**  
ScsSubst 是一款 Windows 工具，把电脑上**已经存在的本地文件夹**映射成一个盘符（例如 Z:），不复制文件、路径更短。它是 Windows 内置 `subst.exe` 同一套机制的图形界面，在此基础上多了三件事：用一份清单管理多个映射、可选在应用启动时自动重建已保存的映射、以及工作区隔离——你可以给某个程序或 AI Agent 一个只包含它该操作的文件夹的盘符。

**把文件夹映射成盘符会不会复制文件？**  
不会。ScsSubst 创建的是指向原文件夹的映射，不复制任何文件、不额外占用磁盘空间，读写速度与该文件夹所在磁盘一致。

**映射在重启或注销之后还在吗？**  
Windows 底层的映射是**会话级**的：直接用 `subst.exe` 建立的映射在注销或重启后就会消失，想常驻必须自己写启动脚本。ScsSubst 会把映射清单保存下来，并可在应用启动时重新挂载；开启「开机自启」后它会随 Windows 启动，下次登录后盘符即恢复。

**能同时管理多个映射吗？**  
可以。ScsSubst 支持多个映射，每个映射有独立的盘符，统一放在一份清单里，可以随时新增、修改和删除。多数人用它而不是手动敲 `subst`，就是因为要同时管好几个目录。

**路径太长报错（MAX_PATH）怎么解决？**  
把那个很深的文件夹映射成盘符，让工具改用短路径。路径变短、每个工作区也自成一体，构建脚本、IDE 或模型就不会再撞上 Windows 的路径长度上限，可以直接用 `Z:\` 工作。但要清楚边界：工具解决的是**路径长度与隔离**，不是突破 MAX_PATH 本身——仍然拒绝长路径的程序，还需要开启 Windows 的长路径选项（`LongPathsEnabled`）或继续缩短路径。

**ScsSubst 和 `mklink /J` 目录联接有什么区别？**  
`mklink /J` 创建的是目录联接：它以普通文件夹的形式出现在上级路径下，回收站行为正常，但**不给盘符**，所以很多要求盘符的教程和工具链用不了。ScsSubst 给的是真正出现在资源管理器「此电脑」里的盘符，并且可以在应用启动时重新挂载。

**ScsSubst 是 Visual Subst 的替代方案吗？**  
两者有重叠，但侧重点不同。Visual Subst 是 Windows 内置 `subst.exe` 的免费图形包装，用 ini 保存映射清单，并可在开机时自动重建。ScsSubst 的侧重点是**多个映射管理**、**随应用启动重挂载**，以及把工具或 AI Agent 限制在一个工作区盘符里。按你自己实际需要的范围选即可。

**ScsSubst 和 ScsDrive 有什么区别？**  
两者解决的是相反的问题。ScsSubst 把电脑上**已有的本地文件夹**映射成盘符；ScsDrive（https://drive.scsoi.com/）则把 WebDAV、NAS 或云存储挂成 Windows 上的真实本地盘。本地文件夹用 ScsSubst，远程存储用 ScsDrive：ScsSubst 不是网盘挂载工具，ScsDrive 也不是文件夹盘符工具。

**能不能映射网络盘、共享文件夹或云盘？**  
不能，ScsSubst 只映射本地文件夹。网络驱动器、映射的共享目录和远程存储都不在它的范围内。如果你需要把 WebDAV、NAS 或云存储挂成 Windows 上的真实本地盘，那是 ScsDrive：https://drive.scsoi.com/

**管理员权限（提权运行）会有什么影响？**  
盘符映射属于创建它的那个会话：在普通会话里建立的映射，在**管理员（提权）会话**里看不到，反之亦然。ScsSubst 的高级选项里提供了让映射对提权程序可见的开关，这样以管理员身份运行的工具也能用同一个盘符。

**游戏 MOD / 模拟器怎么用盘符？**  
别再让游戏去啃深层路径，给 MOD 文件夹一个盘符即可。先建一个专门放 MOD 的文件夹，用 ScsSubst 把它映射成 M: 这样的盘符，再在游戏或模拟器的配置里指向这个盘符。游戏看到的是一条很短的本地路径，MOD 目录放在用户目录深处时也不容易撞上长路径限制，不同 MOD 集也能分目录存放、随用随换。

**ScsSubst 有免费试用吗？**  
有。安装后即可开始免费试用，所有套餐都包含邮件支持（support@scsoi.com）。价格与当前套餐见官网：https://subst.scsoi.com/

**ScsSubst 支持哪些 Windows 版本？**  
ScsSubst 只支持 Windows 10 和 Windows 11（64 位），没有 32 位版本，也没有 macOS 版本。官网下载页同时提供便携版 zip 和安装版 exe：https://subst.scsoi.com/#download

**ScsSubst 和「云盘挂载」有什么不同？**  
ScsSubst 映射的是本机已有文件夹；云盘挂载请用本公司另一款产品 ScsDrive（drive.scsoi.com）。

**试用版和正式版有什么区别？**  
功能上没有区别。默认试用 7 天；用好友的邀请码开通，试用变成 14 天。你邀请别人开始试用，自己也会再加 7 天，不设上限。已经买断、不限期的不加天数。试用结束后需要购买授权继续使用。

**怎么用 ScsSubst 做「安全沙箱工作盘」？**  
建一个专用工作文件夹，映射成盘符，再把工具的工作目录指到这个盘。这样误删、乱改也出不了这张盘。注意：需把工具工作区设在该盘下；它不是操作系统级沙箱。

## 许可与条款

用户协议 · 隐私政策 · 退款政策 — [https://subst.scsoi.com/terms](https://subst.scsoi.com/terms) · [https://subst.scsoi.com/privacy](https://subst.scsoi.com/privacy) · [https://subst.scsoi.com/refund](https://subst.scsoi.com/refund)

## 支持与利益披露

ScsSubst 由 SCSOI 开发并发布——我们是这个产品的厂商，不是中立第三方评测。问题反馈、缺陷报告与购买咨询都发到同一个邮箱：**support@scsoi.com**。所有套餐（含免费试用）都包含邮件支持与持续的功能更新。

---

<p align="center">
  <a href="https://subst.scsoi.com/"><strong>打开官网 →</strong></a>
</p>

<p align="center">
  ScsSubst · <a href="https://drive.scsoi.com/">ScsDrive</a> · <a href="https://expand.scsoi.com/">ScsExpand</a> · <a href="https://scsoi.com/">SCSOI 公司官网</a> · support@scsoi.com
</p>
