# RustMIRAGEOLD

> **Official Forum / 官方论坛**: https://discord.gg/qslab

## Languages

[English](#en) · [中文](#zh)

<a id="en"></a>
## English

### Project Overview

`RustMIRAGEOLD` uses a broad multi-root layout instead of a single compact source root.

The project groups together multiple root-level branches, support libraries, companion trees, and locally preserved work areas in one workspace.

### What This Project Does

At a high level, `RustMIRAGEOLD` works as a multi-branch source archive and workspace. Instead of forcing every part into one main tree, it keeps several parallel areas at the root:

- authentication-related content
- bypass/support branches
- low-level roots
- rendering-related roots
- alternate implementation lines
- bundled support libraries
- additional side work areas

This kind of layout is useful when one project history or one workspace needs to preserve multiple directions side by side instead of collapsing everything into a single unified structure.

### High-Level Design

The project is organized by branch separation rather than by one central application root:

1. major concerns are split into independent root directories
2. specialized trees such as `Render/`, `Auth/`, and `bypass/` keep their own internal subdivision
3. alternate lines such as `mirage/`, `miragerust/`, and `rust/` remain parallel
4. support content such as `freetype/` and `spotify shi/` stays embedded in the same workspace

The result is an archive-style project layout where the root directory itself acts as the main map.

### Root Directory Layout

The root contains:

- `Auth/`
- `bypass/`
- `freetype/`
- `KDMapper/`
- `kernel/`
- `mirage/`
- `miragerust/`
- `Render/`
- `rust/`
- `spotify shi/`
- `src/`
- `unity/`
- `README.md`

This root-level spread defines the overall shape of the project.

### `Auth/`

`Auth/` contains:

- `prot/`

This branch is the authentication-oriented subtree of the workspace.

### `bypass/`

`bypass/` contains:

- `binary/`
- `exploit/`
- `hde/`
- `utils/`

It also includes visible files such as:

- `binary/bytes.h`

This branch is one of the most internally subdivided root trees in the project.

### `freetype/`

`freetype/` contains:

- `include/`
- `win64/`

Inside `include/`, the visible nested directory is:

- `freetype/`

This subtree provides bundled support/dependency content directly at the workspace root.

### `KDMapper/`

`KDMapper/` is a standalone root-level module area. In the currently visible extracted tree, no deeper first-level child directories are shown.

### `kernel/`

`kernel/` is a standalone root-level low-level area.

### `mirage/`

`mirage/` contains:

- `loop/`

This branch keeps its own internal subtree under a separate root-level area.

### `miragerust/`

`miragerust/` contains:

- `x64/`

Inside `x64/`, the visible nested directory is:

- `Debug/`

This branch preserves its own local output-oriented subtree.

### `Render/`

`Render/` contains:

- `imgui/`
- `overlay/`

This branch is clearly dedicated to rendering-oriented project content and is internally split between UI/rendering support and overlay-facing content.

### `rust/`

`rust/` contains:

- `caches/`

This root-level branch adds another separate implementation/support area to the workspace.

### `spotify shi/`

`spotify shi/` contains:

- `curl-for-windows/`
- `json/`
- `stuff/`

Inside `curl-for-windows/`, the visible nested directories include:

- `curl/`
- `openssl/`
- `out/`
- `zlib/`

Inside `stuff/`, the visible nested directories include:

- `.github/`
- `data/`
- `deprecated/`
- `docs/`
- `stb_image_resize_test/`
- `tests/`
- `tools/`

This root-level subtree is one of the broadest side branches in the workspace.

### `src/`

`src/` is present as a traditional source directory at the root. The project keeps `src/` alongside many other top-level trees instead of using it as the only main entry path.

### `unity/`

`unity/` is another standalone root-level branch. In the current extracted tree, deeper first-level child directories are not shown.

### Project Organization

The workspace groups together:

- authentication-oriented content
- a heavily subdivided `bypass/` tree
- standalone low-level module roots
- `mirage` / `miragerust` / `rust` parallel branches
- a rendering-focused root tree
- bundled support/dependency trees
- additional preserved work areas such as `spotify shi/`

The directory names define the project map more strongly than a single root application entry point.

### Build and Output Footprint

The workspace keeps local output-oriented directories in multiple places, including:

- `miragerust/x64/`
- `miragerust/x64/Debug/`
- `freetype/win64/`
- `spotify shi/curl-for-windows/out/`

This preserves the shape of a working local archive rather than a minimal source-only tree.

### Recommended Reading Order

Recommended reading order:

1. `Auth/`
2. `Auth/prot/`
3. `bypass/`
4. `bypass/binary/`
5. `bypass/exploit/`
6. `bypass/hde/`
7. `bypass/utils/`
8. `freetype/`
9. `freetype/include/`
10. `kernel/`
11. `KDMapper/`
12. `mirage/`
13. `mirage/loop/`
14. `miragerust/`
15. `miragerust/x64/`
16. `Render/`
17. `Render/imgui/`
18. `Render/overlay/`
19. `rust/`
20. `rust/caches/`
21. `src/`
22. `unity/`
23. `spotify shi/`
24. `spotify shi/curl-for-windows/`
25. `spotify shi/stuff/`

### Summary

`RustMIRAGEOLD` is a multi-root workspace that includes:

- an authentication branch under `Auth/`
- a subdivided `bypass/` tree
- separate low-level roots such as `kernel/` and `KDMapper/`
- parallel `mirage/`, `miragerust/`, and `rust/` branches
- a rendering tree under `Render/`
- bundled support content such as `freetype/`
- an additional broad side branch under `spotify shi/`

<a id="zh"></a>
## 中文

### 项目概览

`RustMIRAGEOLD` 采用宽型多根目录布局，而不是单一紧凑的源码根目录。

整个项目把多条根级分支、支持库、配套树以及本地保留的工作区内容放进了同一个工作空间。

### 项目作用

从工程层面看，`RustMIRAGEOLD` 更像一个多分支源码归档和工作区。它没有强行把所有内容压进一棵主树，而是在根目录并列保留了多块区域：

- 认证相关内容
- bypass / 支持分支
- 低层根目录
- 渲染相关根目录
- 替代实现线
- bundled 支持库
- 额外的侧向工作区

这种布局适合在一个项目历史或一个工作空间里，同时保留多条方向，而不是把一切收缩成统一结构。

### 整体原理

整个项目采用“按分支隔离”而不是“按单一应用根目录”来组织：

1. 主要关注点被拆成独立的根级目录
2. `Render/`、`Auth/`、`bypass/` 这类专门子树保留自己的内部拆分
3. `mirage/`、`miragerust/`、`rust/` 这类替代实现线保持并列
4. `freetype/`、`spotify shi/` 等支持内容直接嵌在同一个工作区里

最终形成的是一种偏归档式布局：根目录本身就是整个项目最重要的地图。

### 根目录结构

根目录包含：

- `Auth/`
- `bypass/`
- `freetype/`
- `KDMapper/`
- `kernel/`
- `mirage/`
- `miragerust/`
- `Render/`
- `rust/`
- `spotify shi/`
- `src/`
- `unity/`
- `README.md`

这些根级目录共同定义了整个项目的形态。

### `Auth/`

`Auth/` 包含：

- `prot/`

这一分支对应工作区中的认证相关子树。

### `bypass/`

`bypass/` 包含：

- `binary/`
- `exploit/`
- `hde/`
- `utils/`

同时还能看到：

- `binary/bytes.h`

这一分支是项目中内部拆分最明显的根级树之一。

### `freetype/`

`freetype/` 包含：

- `include/`
- `win64/`

在 `include/` 内部，可见的嵌套目录为：

- `freetype/`

这一子树把 bundled 支持/依赖内容直接放在工作区根部。

### `KDMapper/`

`KDMapper/` 是独立的根级模块区域。在当前提取树中没有展示更深的一级子目录。

### `kernel/`

`kernel/` 是独立的根级低层区域。

### `mirage/`

`mirage/` 包含：

- `loop/`

这一分支在独立的根级区域下保留了自己的内部子树。

### `miragerust/`

`miragerust/` 包含：

- `x64/`

在 `x64/` 内部，可见的嵌套目录为：

- `Debug/`

这一分支保留了自己的本地输出导向子树。

### `Render/`

`Render/` 包含：

- `imgui/`
- `overlay/`

这一分支明确对应渲染相关项目内容，并且内部继续拆分为 UI/渲染支持区和 overlay 区域。

### `rust/`

`rust/` 包含：

- `caches/`

这一根级分支为工作区增加了另一块独立实现/支持区域。

### `spotify shi/`

`spotify shi/` 包含：

- `curl-for-windows/`
- `json/`
- `stuff/`

在 `curl-for-windows/` 内部，可见的嵌套目录包括：

- `curl/`
- `openssl/`
- `out/`
- `zlib/`

在 `stuff/` 内部，可见的嵌套目录包括：

- `.github/`
- `data/`
- `deprecated/`
- `docs/`
- `stb_image_resize_test/`
- `tests/`
- `tools/`

这一根级子树是整个工作区中体量较大的侧向分支之一。

### `src/`

`src/` 以传统源码目录的形式存在于根部，但项目并没有把它作为唯一主入口，而是与许多其他顶层树并列保留。

### `unity/`

`unity/` 是另一棵独立的根级分支。在当前提取树中没有展示更深的一级子目录。

### 项目组织方式

整个工作区把以下内容组合在一起：

- 认证相关内容
- 内部继续拆分的 `bypass/` 树
- 独立的低层模块根目录
- 平行存在的 `mirage` / `miragerust` / `rust` 分支
- 渲染专用根级树
- bundled 支持/依赖树
- 诸如 `spotify shi/` 这样的额外保留工作区

目录名本身比单一主应用入口更能定义整个项目地图。

### 构建与输出痕迹

工作区在多个位置保留了本地输出导向目录，包括：

- `miragerust/x64/`
- `miragerust/x64/Debug/`
- `freetype/win64/`
- `spotify shi/curl-for-windows/out/`

这些目录让整个项目保留了真实本地归档工作树的形态，而不是最小源码树。

### 阅读建议

推荐按下面顺序阅读：

1. `Auth/`
2. `Auth/prot/`
3. `bypass/`
4. `bypass/binary/`
5. `bypass/exploit/`
6. `bypass/hde/`
7. `bypass/utils/`
8. `freetype/`
9. `freetype/include/`
10. `kernel/`
11. `KDMapper/`
12. `mirage/`
13. `mirage/loop/`
14. `miragerust/`
15. `miragerust/x64/`
16. `Render/`
17. `Render/imgui/`
18. `Render/overlay/`
19. `rust/`
20. `rust/caches/`
21. `src/`
22. `unity/`
23. `spotify shi/`
24. `spotify shi/curl-for-windows/`
25. `spotify shi/stuff/`

### 总结

`RustMIRAGEOLD` 是一个多根目录工作区，包含：

- 位于 `Auth/` 下的认证分支
- 内部继续拆分的 `bypass/` 树
- 独立的低层根目录，如 `kernel/` 与 `KDMapper/`
- 平行存在的 `mirage/`、`miragerust/` 与 `rust/` 分支
- 位于 `Render/` 下的渲染树
- 位于 `freetype/` 下的 bundled 支持内容
- 位于 `spotify shi/` 下的额外大型侧向分支
