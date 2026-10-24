[English](README.md) · **中文** · [日本語](README.ja.md) · [한국어](README.ko.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)

<p align="center">
  <img src="docs/banner.svg" alt="ScsSubst" width="100%">
</p>

<h1 align="center">ScsSubst</h1>

<p align="center">
  <strong>把文件夹变成盘符</strong><br>
  给深层目录一个盘符入口，不复制文件，像本地硬盘一样打开。
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
  <a href="https://github.com/shuyingegit/scssubst/releases"><strong>发行版</strong></a> ·
  <a href="https://drive.scsoi.com"><strong>ScsDriver</strong></a>
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

- **一键挂载** — 选择文件夹与盘符，一点「连接」即可映射，开机可自动恢复。
- **本地体验** — 在资源管理器里像普通盘符一样使用，路径更短更好记。
- **开机自启** — 打开软件时可自动挂载已保存的映射项。
- **轻量稳定** — 纯系统 API，不捆绑第三方文件系统驱动，绿色包体积小。
- **多服务器** — 可添加多条映射，各自独立盘符，互不干扰。
- **安全连接** — 可选「管理员程序可见」、回收站等高级选项，默认保持简单。
- **安装即试用** — 默认 7 天试用；到期后用授权码激活（月 / 年 / 终身）。
- **沙箱工作盘** — 会写盘的工具常越界乱删。给它单独工作目录并映射成盘符，工作区指到该盘——越界也出不了这张盘。


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

## 姊妹产品

把 WebDAV / 网盘 挂成 Windows 本地磁盘，像本地硬盘一样打开云端文件。

→ **[ScsDrive](https://github.com/shuyingegit/scsdriver)** · [drive.scsoi.com](https://drive.scsoi.com)

## 常见问题

**ScsSubst 和「云盘挂载」有什么不同？**  
ScsSubst 映射的是本机已有文件夹；云盘挂载请用本公司另一款产品 ScsDriver（drive.scsoi.com）。

**试用版和正式版有什么区别？**  
功能上没有区别。默认试用 7 天；用好友的邀请码开通，试用变成 14 天。你邀请别人开始试用，自己也会再加 7 天，不设上限。已经买断、不限期的不加天数。试用结束后需要购买授权继续使用。

**怎么用 ScsSubst 做「安全沙箱工作盘」？**  
建一个专用工作文件夹，映射成盘符，再把工具的工作目录指到这个盘。这样误删、乱改也出不了这张盘。注意：需把工具工作区设在该盘下；它不是操作系统级沙箱。

## 许可与条款

用户协议 · 隐私政策 · 退款政策 — [https://subst.scsoi.com/terms](https://subst.scsoi.com/terms) · [https://subst.scsoi.com/privacy](https://subst.scsoi.com/privacy) · [https://subst.scsoi.com/refund](https://subst.scsoi.com/refund)

---

<p align="center">
  <a href="https://subst.scsoi.com/"><strong>打开官网 →</strong></a>
</p>
