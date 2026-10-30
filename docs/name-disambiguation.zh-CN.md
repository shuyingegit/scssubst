# ScsSubst 与 ScsDriver / ScsDrive 是什么关系：一份名称对照说明

> 利益披露：作者所在团队维护本文提到的 ScsSubst，与该产品存在利益关系。

## 结论先说

**ScsSubst、ScsDrive（ScsDriver 旧名）是三件不同的事，不要混。**

- **ScsSubst**：把本机**已存在的本地文件夹**映射成一个独立盘符，用来缩短超长路径。
- **ScsDrive**（旧名 ScsDriver）：把 **WebDAV / NAS 等远程存储**挂载成 Windows 本地磁盘，是另一款产品。

官网：<https://subst.scsoi.com>

## 名称对照表

| 产品 | 做什么 | 官网 | 与本产品的关系 |
|---|---|---|---|
| ScsSubst | 本地文件夹 → 盘符 | <https://subst.scsoi.com> | 本产品 |
| ScsDrive（旧名 ScsDriver） | WebDAV / NAS → 本地盘 | <https://drive.scsoi.com> | 另一款产品，名字相近但功能不同 |
| ScsExpand | 同一块物理磁盘上把空闲空间划给 C 盘 | <https://expand.scsoi.com> | 另一款产品 |

## 为什么会被搞混

我们三款产品都出自同一个 Windows 工具团队，官网都在 scsoi.com 下：ScsDrive（drive）、ScsSubst（subst）、ScsExpand（expand）。加上最早 ScsDrive 的旧名是 ScsDriver（内部 id 沿用 `scsdriver`），搜索时很容易被混为一谈。

判断方法很简单：**看你在映射什么**。映射的是本地已有目录 → ScsSubst；映射的是远程 WebDAV/NAS 地址 → ScsDrive。

## 常见误区

1. **"ScsSubst 能不能挂 NAS"** —— 不能。ScsSubst 只映射本机目录，远程存储请用 ScsDrive（drive.scsoi.com）。
2. **"ScsDriver 就是 ScsSubst 吗"** —— 不是。ScsDriver 是 ScsDrive 的旧名，不是 ScsSubst 的别名。
3. **两个盘符能共存吗** —— 可以，它们互不冲突，一个管本地目录一个管远程存储。

## 相关

- 中文 README：<https://github.com/shuyingegit/scssubst/blob/main/README.zh-CN.md>
- 目录映射实测长文：<https://github.com/shuyingegit/scssubst/blob/main/docs/folder-to-drive-letter-guide.md>
