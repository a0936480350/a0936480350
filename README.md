# 👋 Hi, I'm Mike

物流系統開發工程師 + **10 年音樂老師** + 持續轉型全端 SaaS 開發
主要使用 C# / ASP.NET Core / PostgreSQL，擅長把真實業務需求變成可上線、可長期營運的產品。

![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=c-sharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET_8-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-5C2D91?style=flat-square&logo=.net&logoColor=white)
![EF Core](https://img.shields.io/badge/EF_Core-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoft-sql-server&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![SignalR](https://img.shields.io/badge/SignalR-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![WPF](https://img.shields.io/badge/WPF-0078D6?style=flat-square&logo=windows&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Bicep](https://img.shields.io/badge/Bicep-0080FF?style=flat-square&logo=microsoftazure&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

---

## 🌟 作品集（點進去看完整介紹）

### 🚀 [LeadFlow.SaaS — 音樂教室營運中台](https://github.com/a0936480350/LeadFlow.SaaS) · 現役旗艦

> 把音樂教室的「招生 → 排課 → 點名 → 學習筆記 → 主管總覽」全打通的多租戶 SaaS。第一個客戶就是我自己的音樂教室（dogfooding 中）。

| 面向 | 內容 |
|------|------|
| 🌐 **Live** | [leadflow-mike-tw.azurewebsites.net](https://leadflow-mike-tw.azurewebsites.net) |
| 🛠️ **技術棧** | ASP.NET Core 8 MVC · EF Core 8 · **PostgreSQL 16** (Npgsql) · ASP.NET Core Identity · Tailwind + Preline · FullCalendar.js · Serilog · xUnit |
| 🔐 **架構** | **Multi-tenant SaaS**（ITenantContext + EF Global Query Filter + SaveChanges Interceptor 三層防禦）|
| ☁️ **部署** | Azure App Service Linux + PostgreSQL Flexible Server · **Bicep** 一鍵 IaC · GitHub Actions 自動 CI/CD + smoke check |
| 📊 **規模** | 32 milestones (M0+M1+M2 全部交付) · 14 Domain entities · 21 DB tables · 17 Application services · ~50 Views · 70+ commits |
| 🤖 **特色** | 兩個 AI agent（Claude + Codex）平行開發，靠 `.agents/` 資料夾自助協作，零訊息轉述 |

---

### ⭐ [DevLearn — 程式設計學習平台](https://github.com/a0936480350/DevLearn)

> 232 章教學、8 款遊戲化學習、老師媒合、即時聊天、AI 輔助開發。一個人獨立開發 1 個月。

| 面向 | 內容 |
|------|------|
| 🌐 **Live Demo** | [devlearn-dotnet.azurewebsites.net](https://devlearn-dotnet.azurewebsites.net/) |
| 🛠️ **技術棧** | ASP.NET Core 8 MVC · EF Core · PostgreSQL · SignalR · Phaser.js 3 |
| 📊 **規模** | 60+ DB tables · 30+ Controllers · 232 章節 · 500+ 題目 |

---

### 🚗 [CarMaintenanceApp — 車輛保養管理系統](https://github.com/a0936480350/CarMaintenanceApp)

> WPF 桌面應用，完整實作前後台分離的車輛保養紀錄管理系統。真實業務需求。

**亮點：** 前後台分離 · Azure SQL · LiveCharts 圖表 · Bluetooth 硬體整合 · Session 管理
**技術：** C# · WPF · ADO.NET · 32feet.NET

---

### 🎸 [GuitarSurvey — 吉他教學問卷網站](https://github.com/a0936480350/GuitarSurvey)

> ASP.NET Core Razor Pages 作品，吉他課程學員報名問卷系統。

**亮點：** Razor Pages · Model Binding · 參數化 SQL 查詢 · 表單驗證
**技術：** ASP.NET Core 8 · Razor Pages · SQL Server · Bootstrap

---

### 🇯🇵 [JapaneseGames — 日文學習小遊戲](https://github.com/a0936480350/JapaneseGames)

> 兩款 WinForms 日文學習工具：單字記憶遊戲 + 互動問答。從自身日語學習需求出發做的工具。

**亮點：** WinForms · 500+ 內建題庫 · 外部題庫擴充 · 兩版本漸進改善
**技術：** C# · WinForms · .NET 8

---

### 📂 [SideProjects](https://github.com/a0936480350/SideProjects) & [practice-work](https://github.com/a0936480350/practice-work)

> 日常練習與小型專案集合，記錄學習歷程。

---

## 🎓 技術領域

### 後端
- **C#** — OOP、LINQ、async/await、泛型、委派/事件、record、pattern matching
- **ASP.NET Core 8** — MVC、Razor Pages、Web API、SignalR、Middleware、DI 容器、IExceptionHandler
- **ASP.NET Core Identity** — Cookie auth、ClaimsPrincipalFactory 客製、Multi-tenant 整合
- **EF Core 8** — Code First、Migration、Global Query Filter、SaveChanges Interceptor、複合索引、效能優化、N+1 處理
- **SQL** — Query 優化、Index 設計、Stored Procedure、Window Functions
- **ADO.NET** — 直接操作，理解 ORM 抽象層底下的運作

### Multi-Tenant SaaS 架構（LeadFlow 實戰）
- **ITenantContext** — Claim-based tenant 解析
- **EF Global Query Filter** — 自動為每個 tenant-scoped entity 加 `WHERE TenantId = @ctx`
- **SaveChanges Interceptor** — 寫入時自動蓋章 + 阻擋 anonymous 寫入 + 阻擋 tenant 遷移
- **Identity 表豁免** — 登入流程必須能查 user，跨 tenant 列舉由 service 層 gate
- **Reflection-based filter** — 對所有實作 `ITenantScoped` 的 entity 自動掛載

### 前端 / UI
- **Tailwind CSS + Preline UI** — utility-first，CDN-config 對應 CSS 變數
- **FullCalendar.js 6** — 週/月/日視圖、custom event source、衝堂視覺化
- **JavaScript** — ES6+、Promise、Fetch API、Debounced AJAX validation
- **HTML/CSS** — Flexbox、Grid、RWD、動畫效果
- **遊戲開發** — Phaser.js 3
- **即時通訊** — SignalR Client（WebSocket）

### 桌面開發
- **WPF** — XAML、Data Binding、LiveCharts、前後台分離設計
- **WinForms** — 事件驅動、GDI+、控制項自訂
- **硬體整合** — Bluetooth (32feet.NET)、Serial Port

### 架構思維
- **Clean Architecture** — Domain / Application / Infrastructure / Web 嚴格分層
- **SOLID 原則** + **設計模式** — Repository、Strategy、Factory、Observer、Decorator
- **系統設計** — 認證機制（Session/JWT/OAuth/Identity）、快取策略、微服務 vs 單體
- **可觀測性** — Serilog 結構化日誌、RFC 7807 Problem Details、healthcheck endpoints
- **測試策略** — xUnit + WebApplicationFactory 整合測試
- **安全性** — SQL Injection 防禦、XSS、CSRF、密碼雜湊、Tenant 跨界保護

### DevOps / Cloud
- **Azure App Service**（Linux .NET 8）+ **Azure Database for PostgreSQL**（Flexible Server）
- **Bicep IaC** — App Service Plan + Web App + Postgres + firewall 一鍵 provisioning
- **GitHub Actions CI/CD** — push to main → restore + build + test + publish + deploy + smoke check
- **Docker Compose** — 本機 PostgreSQL 開發環境
- **Git** — 分支策略、Rebase vs Merge、團隊協作、SourceTree GUI
- **Conventional Commits** + 嚴格 commit message 規範

---

## 🛠️ 工具與環境

| 類別 | 使用中 |
|------|--------|
| IDE | Visual Studio 2022、VS Code |
| 資料庫 | PostgreSQL、SQL Server、Azure SQL |
| 版控 | Git、GitHub、GitHub Actions |
| 部署 | Azure App Service · Bicep IaC |
| 觀測 | Serilog · Healthcheck endpoints |
| AI 協作 | Claude Code + Codex（兩個 agent 平行協作） |

---

## 📊 作品組合多樣性

| 技術類型 | 代表作 |
|---------|--------|
| **Multi-tenant SaaS** | **LeadFlow.SaaS** |
| **Web MVC** | LeadFlow · DevLearn |
| **Web Razor Pages** | GuitarSurvey |
| **Desktop WPF** | CarMaintenanceApp |
| **Desktop WinForms** | JapaneseGames |
| **即時通訊** | DevLearn (SignalR) |
| **遊戲引擎** | DevLearn (Phaser.js) |
| **ADO.NET 直接操作** | CarMaintenanceApp、GuitarSurvey |
| **EF Core + 多租戶** | LeadFlow |
| **硬體整合** | CarMaintenanceApp (Bluetooth) |
| **CI/CD 自動化** | LeadFlow (Bicep + GH Actions) · DevLearn (GH Actions → Azure) |

---

## 📖 持續學習

透過 DevLearn 平台整理了自己的學習筆記：
- **語法基礎篇**（200+ 章）— C#、SQL、JavaScript、HTML/CSS、Vue、React
- **概念深入篇**（28 章）— 面試常考的觀念：DI、async、REST、系統設計

> 歡迎到 [DevLearn 網站](https://devlearn-dotnet.azurewebsites.net/) 看完整內容！

---

## 📬 聯絡方式

- 💼 GitHub：[@a0936480350](https://github.com/a0936480350)
- 🚀 現役產品：[LeadFlow.SaaS](https://leadflow-mike-tw.azurewebsites.net) · 音樂教室營運中台
- 🌐 學習平台：[DevLearn](https://devlearn-dotnet.azurewebsites.net/)
- 📱 LINE 官方帳號（DevLearn）：[lin.ee/68vD9ZW](https://lin.ee/68vD9ZW)

---

<sub>⭐ 如果你覺得 LeadFlow 或 DevLearn 有幫助，歡迎在 GitHub 給個 Star！</sub>
