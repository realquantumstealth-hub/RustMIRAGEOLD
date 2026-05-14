# RustMIRAGEOLD

## Languages

[English](#en) · [中文](#zh) · [日本語](#ja) · [한국어](#ko) · [Русский](#ru) · [Українська](#uk) · [Tiếng Việt](#vi)

<a id="zh"></a>
## 中文说明

`RustMIRAGEOLD` 是历史版本的反作弊研究工程集合，目录中包含多个子模块（如认证、内核相关、渲染与辅助组件）。

当前结构示例：

- `Auth/`：认证与鉴权相关代码
- `kernel/`、`KDMapper/`、`bypass/`：底层研究与历史实验模块
- `Render/`、`mirage/`、`unity/`：渲染与业务逻辑模块
- `freetype/`、`src/`：依赖与基础代码

### 研究目标

- 归档历史方案，便于版本对比与技术演进复盘
- 分析多模块工程的职责拆分与耦合关系
- 为后续重构和规范化输出提供参考

### 合规与边界

本项目用于研究归档与防御技术讨论，不提供可直接用于实战的敏感能力交付。

由于部分密钥、证书、可执行链路、绕过/注入成品等属敏感信息不方便在 GitHub 上公开，需要或想交流的同伴可以联系我们官方 Discord 进行深入探讨。

---

<a id="en"></a>
## English

`RustMIRAGEOLD` is a legacy anti-cheat research codebase collection containing multiple submodules (authentication, kernel-related, rendering, and support components).

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

Some keys, certificates, executable chains, and bypass/injection deliverables are sensitive and are not suitable for public release on GitHub. For deeper discussion, please contact our official Discord.

---

<a id="ja"></a>
## 日本語

`RustMIRAGEOLD` は過去版のアンチチート研究コードを集約したリポジトリです。認証、カーネル関連、描画、補助モジュールなどを含みます。

構成例：

- `Auth/`：認証関連コード
- `kernel/`、`KDMapper/`、`bypass/`：低レベル研究・過去実験モジュール
- `Render/`、`mirage/`、`unity/`：描画とドメインロジック
- `freetype/`、`src/`：依存と基礎コード

### 研究目的

- 旧アプローチのアーカイブと比較
- マルチモジュール構成の責務分割と結合度分析
- 将来のリファクタリングに向けた基礎資料化

### コンプライアンス

本プロジェクトは研究アーカイブと防御技術議論のみを目的とします。

鍵・証明書・実行チェーン・バイパス/インジェクション成果物などの機微情報は GitHub で公開しません。詳細は公式 Discord へご連絡ください。

---

<a id="ko"></a>
## 한국어

`RustMIRAGEOLD`는 구버전 안티치트 연구 코드 모음 저장소입니다. 인증, 커널 관련, 렌더링, 보조 모듈 등이 포함됩니다.

구성 예시:

- `Auth/`: 인증 관련 코드
- `kernel/`, `KDMapper/`, `bypass/`: 저수준 연구/과거 실험 모듈
- `Render/`, `mirage/`, `unity/`: 렌더링 및 도메인 로직
- `freetype/`, `src/`: 의존성 및 기본 코드

### 연구 목표

- 과거 접근 방식 아카이브 및 버전 비교
- 멀티 모듈 구조의 책임 분리와 결합도 분석
- 향후 리팩터링/정규화 작업을 위한 참고 자료 제공

### 준수 및 범위

본 프로젝트는 연구 아카이브 및 방어 기술 논의를 위한 용도입니다.

키, 인증서, 실행 체인, 바이패스/인젝션 결과물 등 민감 정보는 GitHub에 공개하지 않습니다. 자세한 논의는 공식 Discord로 문의해 주세요.

---

<a id="ru"></a>
## Русский

`RustMIRAGEOLD` — коллекция legacy-кода для исследований anti-cheat. Включает подсистемы аутентификации, kernel-части, рендеринг и вспомогательные модули.

Пример структуры:

- `Auth/`: код аутентификации
- `kernel/`, `KDMapper/`, `bypass/`: низкоуровневые исследования и исторические эксперименты
- `Render/`, `mirage/`, `unity/`: рендеринг и доменная логика
- `freetype/`, `src/`: зависимости и базовый код

### Цели исследования

- Архивирование legacy-подходов и сравнение версий
- Анализ разделения ответственности и связности модулей
- Подготовка базы для будущего рефакторинга

### Соответствие и ограничения

Проект предназначен для архивных исследований и defensive-дискуссий.

Ключи, сертификаты, исполняемые цепочки и готовые bypass/injection материалы не публикуются на GitHub. Для обсуждения используйте официальный Discord.

---

<a id="uk"></a>
## Українська

`RustMIRAGEOLD` — це колекція legacy-коду для anti-cheat досліджень. Містить підсистеми автентифікації, kernel-частини, рендеринг і допоміжні модулі.

Приклад структури:

- `Auth/`: код автентифікації
- `kernel/`, `KDMapper/`, `bypass/`: низькорівневі дослідження та історичні експерименти
- `Render/`, `mirage/`, `unity/`: рендеринг і доменна логіка
- `freetype/`, `src/`: залежності та базовий код

### Мета дослідження

- Архівування legacy-підходів і порівняння версій
- Аналіз розподілу відповідальностей і зв’язаності модулів
- Підготовка основи для майбутнього рефакторингу

### Відповідність і межі

Проєкт призначено для архівних досліджень і defensive-обговорень.

Ключі, сертифікати, виконувані ланцюги та готові bypass/injection матеріали не публікуються на GitHub. Для обговорення використовуйте офіційний Discord.

---

<a id="vi"></a>
## Tiếng Việt

`RustMIRAGEOLD` là bộ sưu tập mã legacy cho nghiên cứu anti-cheat. Bao gồm mô-đun xác thực, phần kernel, render và các thành phần hỗ trợ.

Ví dụ cấu trúc:

- `Auth/`: mã xác thực
- `kernel/`, `KDMapper/`, `bypass/`: nghiên cứu mức thấp và mô-đun thử nghiệm lịch sử
- `Render/`, `mirage/`, `unity/`: render và logic nghiệp vụ
- `freetype/`, `src/`: phụ thuộc và mã nền tảng

### Mục tiêu nghiên cứu

- Lưu trữ cách tiếp cận legacy và so sánh phiên bản
- Phân tích tách trách nhiệm và mức độ kết dính mô-đun
- Làm tài liệu tham chiếu cho refactor trong tương lai

### Tuân thủ và phạm vi

Dự án dùng cho lưu trữ nghiên cứu và thảo luận kỹ thuật phòng thủ.

Một số khóa, chứng chỉ, chuỗi thực thi và sản phẩm bypass/injection là thông tin nhạy cảm nên không công khai trên GitHub. Nếu cần trao đổi sâu hơn, vui lòng liên hệ Discord chính thức của chúng tôi.
