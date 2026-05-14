# RustMIRAGEOLD

## Language / 语言

| Language | Jump |
| --- | --- |
| 简体中文 | [查看中文](#中文说明) |
| English | [View English](#english) |

## 中文说明

`RustMIRAGEOLD` 是历史版本的反作弊研究工程集合，目录中包含多个子模块（如认证、内核相关、渲染与辅助组件）。

当前结构示例：

- `Auth/`：认证与鉴权相关代码
- `kernel/`、`KDMapper/`、`bypass/`：低层研究与历史实验模块
- `Render/`、`mirage/`、`unity/`：渲染与业务逻辑模块
- `freetype/`、`src/`：依赖与基础代码

### 研究目标

- 归档历史方案，便于版本对比与技术演进复盘
- 分析多模块工程的职责拆分与耦合关系
- 为后续重构和规范化输出提供参考

### 合规与边界

本项目用于研究归档与防御技术讨论，不提供可直接用于实战的敏感能力交付。

**由于部分密钥、证书、可执行链路、绕过/注入成品等属敏感信息不方便在github上公开，需要或想交流的同伴可以联系我们官方discord进行深入探讨。**

---

## English

`RustMIRAGEOLD` is a legacy anti-cheat research codebase collection, containing multiple submodules (authentication, kernel-related, rendering, and support components).

Current structure example:

- `Auth/`: authentication-related code
- `kernel/`, `KDMapper/`, `bypass/`: low-level research and historical experiment modules
- `Render/`, `mirage/`, `unity/`: rendering and domain logic modules
- `freetype/`, `src/`: dependencies and base code

### Research Focus

- Archive legacy approaches for version comparison and evolution review
- Analyze responsibility split and coupling across multi-module systems
- Provide references for future refactoring and standardization

### Compliance & Boundaries

This project is for research archiving and defensive technical discussion only, and does not provide directly deployable sensitive capabilities.

**Some keys, certificates, executable chains, and bypass/injection deliverables are sensitive and are not suitable for public release on GitHub. If you need deeper discussion, please contact our official Discord.**



