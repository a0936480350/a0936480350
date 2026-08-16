<!--
  GitHub profile README · 2026-08-16 update
  ─────────────────────────────────────────
  This version preserves Mike's existing structure (DevLearn /
  CarMaintenance / Japanese / side projects all kept) and only
  refreshes the LeadFlow headline section to match reality after
  three more months of shipped work (teacher invite links, 3-way
  session completion confirmation, onboarding flow guide, and a
  round of bug fixes/hardening).

  Deploy flow:
  1. Open https://github.com/a0936480350/a0936480350 (the profile repo)
  2. Edit README.md → paste everything below (replacing whole file)
  3. Commit → github.com/a0936480350 updates instantly
-->

## 👋 Hi, I'm Mike

全端工程師 + **10 年音樂老師** + **6 年日本與在台日商業務**  
主力 C# / ASP.NET Core / PostgreSQL，擅長把真實業務需求變成可上線、可長期營運的產品。  
2026 年起延伸到 **iOS（Swift + Vision）** 與 **瀏覽器端訊號處理**，做「用鏡頭與麥克風即時判斷動作對錯」的教學工具。

![C#](https://img.shields.io/badge/C%23_12-239120?style=flat-square&logo=csharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET_8-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![ASP.NET](https://img.shields.io/badge/ASP.NET_Core-5C2D91?style=flat-square&logo=dotnet&logoColor=white)
![EF Core](https://img.shields.io/badge/EF_Core_8-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL_16-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![SignalR](https://img.shields.io/badge/SignalR-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Swift](https://img.shields.io/badge/Swift_5-FA7343?style=flat-square&logo=swift&logoColor=white)
![Vision](https://img.shields.io/badge/Apple_Vision-000000?style=flat-square&logo=apple&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-0097A7?style=flat-square&logo=google&logoColor=white)
![Web Audio](https://img.shields.io/badge/Web_Audio_API-FF6F00?style=flat-square&logo=javascript&logoColor=white)
![WPF](https://img.shields.io/badge/WPF-0078D4?style=flat-square&logo=windows&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Bicep](https://img.shields.io/badge/Bicep-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

---

## 🌟 作品集（點進去看完整介紹）

### 🚀 [LeadFlow.SaaS — 教務管理中台（音樂 / 才藝 / 補教）](https://leadflow-mike-tw.azurewebsites.net/) · 現役旗艦

把教室的「**招生 → 官網 → 排課 → 點名 → 堂數 → 薪資 → 家長通知 → 月報 → 線上收費**」全打通的多租戶 SaaS。第一個客戶就是我自己的音樂教室（dogfooding 中）。

**🌐 Live:** [leadflow-mike-tw.azurewebsites.net](https://leadflow-mike-tw.azurewebsites.net/)　·　原始碼私有（商業產品）

**🛠️ 技術棧：** ASP.NET Core 8 MVC · EF Core 8 · PostgreSQL 16 (Npgsql) · ASP.NET Core Identity · LINE Login (manual OAuth2) · MailKit + Gmail SMTP · 綠界 ECPay (SHA256 V5) · Tailwind + Preline · FullCalendar.js 6 · Serilog · xUnit

**🔐 架構：** Multi-tenant SaaS（ITenantContext + EF Global Query Filter + SaveChanges Interceptor 三層防禦）· Per-tenant Feature Flag 系統（RFC 0010）

**☁️ 部署：** Azure App Service Linux + PostgreSQL Flexible Server · Bicep 一鍵 IaC · GitHub Actions 自動 CI/CD + smoke check · Auto-migrate on startup

**📊 規模：** M1–M4.30+ · **577** commits · **35** Domain entities · **30+** EF migrations · **48** Application services · **55** Controllers · **165** Views · **60+** xUnit tests 全綠 · **17** RFC 決策文件

**✨ 核心功能（都已上線）：**
- 🗓️ 排課日曆（30 分鐘格 · 衝堂偵測 · 批次排課 · 教室資源）
- 🧾 堂數管理（預約式扣堂 · 缺席 3 政策 · 補課期限 · 套餐生命週期 RFC 0009）
- ✅ 三方課堂完成確認（老師 / 學生・家長各自標記，教室最終確認才計入薪資，教室永遠保有最終確認權）
- 💰 老師薪資（三種抽成模式 · 已上完 vs 預估分開 · CSV 匯出）
- 👨‍👩‍👧 家長 Portal（LINE 綁定登入 · 課表 · 堂數 · 歷史月報 · 一鍵請假 · 完成確認）
- 👩‍🏫 老師 Portal（獨立帳號 · 今日課表 · 打卡 · 空堂時間表 · 我的薪資）
- ✉️ 老師邀請免 Email 加入（連結手動分享，接受時再補真實 Email，降低教室導入門檻）
- 📧 自動通知（學習筆記 email · 課前 24 小時提醒 · 每月學習報告自動生成 · 公開官網 lead 即時通知，可開關）
- 🔴 未讀 Lead 導覽列 badge（24 小時窗口自動淡出，不用手動推進 stage）
- 💳 線上訂閱（綠界 ECPay V5 · 月/季/年付 · 過期自動降級）
- 🎚️ Per-tenant 客製化（Feature Flag · Tier B/C 加購功能即時開關）
- 🎨 白牌官網（3 版型 · 表單直通後台 · Tenant 自訂品牌色 / Logo · 老師 / 課程 / 場地照片渲染 · Google 地圖導航）
- 📸 照片上傳（老師 / 學生 / 課程 / 教室場地 · Azure 持久化儲存 · 公開頁 + 列表 + 詳情多處顯示）
- 📎 筆記教材附件（PDF 樂譜 / 作業照片 · 10MB/檔 · 多檔批次上傳 · 圖片預覽 + PDF 下載）
- 📘 三端快速操作流程指南（教室老闆 / 老師 / 學生・家長，內建 Help 頁）

**🤖 特色：** 兩個 AI agent（Claude + Codex）平行開發，靠 `.agents/` 資料夾自助協作，零訊息轉述 · RFC-first 決策流程 · 每次 push 自動跑測試 + Smoke check

---

### 🇯🇵 Nihon-Dev — 台灣工程師日本求職平台

獨立設計並開發的 Blazor Server 全端平台，幫台灣工程師準備日本求職（履歷格式、技術日文、面試流程）。

**🌐 Live:** [nihon-dev-20260419.azurewebsites.net](https://nihon-dev-20260419.azurewebsites.net)

**🛠️ 技術棧：** Blazor Server · EF Core · PostgreSQL · Google Gemini API · 綠界 ECPay · GitHub Actions → Azure App Service

**✨ 重點：**
- 會員系統、內容管理、多角色權限（學員 / 老師 / 管理員）
- 串接 Google Gemini API 做 AI 詞彙解釋，含多模型 quota 自動 fallback、cookie-based rate limiting（免費 / 付費方案分流）
- 100+ 篇日本 IT 求職相關教材內容

---

### 🏋️ [ElasticBandCoach — 給長輩的坐姿彈力帶教練](https://github.com/a0936480350/elastic-band-coach) · iOS / Mac

給爸爸做的。鏡頭偵測骨架 → 算關節角度 → 判斷姿勢標不標準 → 畫面跳大字＋語音講出來要修哪裡。
**全程在裝置上運算，影像不儲存、不上傳、不需要網路。**

**🛠️ 技術棧：** Swift · UIKit · Apple Vision（`VNDetectHumanBodyPoseRequest` 19 點骨架）· AVFoundation · AVSpeechSynthesizer · My Mac (Designed for iPad)

**📊 規模：** 30 個 Swift 檔 · 2,906 行 · 8 個動作定義 · 一週三天課表

**✨ 幾個刻意的設計：**
- **所有量測除以肩寬正規化** —— 人靠近或退後鏡頭，判斷數值都不會跑掉
- **一次只講一句話** —— 同時給三個指令長輩會直接放棄，所以只播報最該修的那條
- **示範火柴人由關節角度即時繪製**，不用網路影片 —— 示範與評分永遠是同一份定義，不可能走鐘，也沒有版權問題
- 內建模擬人偶，**不用鏡頭也能先看一遍**判斷長什麼樣（第一次拿給長輩看很好用）

---

### 🎸 [Guitar Coach — 吉他練習即時回饋](https://github.com/a0936480350/guitar-coach) · Web

**🌐 Live:** [a0936480350.github.io/guitar-coach](https://a0936480350.github.io/guitar-coach/)

聽你彈得對不對、看你姿勢對不對，再出題考你的耳朵。純前端，**沒有後端、沒有資料庫，影像與聲音不離開裝置**。

**🛠️ 技術棧：** Web Audio API（FFT / chroma / YIN 音高偵測 / Karplus-Strong 撥弦合成）· MediaPipe HandLandmarker · 單應性變換（指板座標對應）· Canvas · 原生 ES modules 零框架

**✨ 功能：** 和弦偵測（33 個和弦三段可選）· 單音 Solo 偵測 · 聽力測驗（音程 / 和弦進行級數 / 和弦組成 / 和弦種類，範圍可複選）· 五線譜 ↔ TAB 切換 · 調音器（誤差 < 1 音分）· 節拍器（三/五/六連音細分）· 鼓機 8 風格 · Full Band 伴奏（6 曲風 × 12 key）· 左手姿勢與指板校準

**🧪 工程重點 —— 沒有樂器也能驗證演算法：**
DSP 核心是純函式，不碰 DOM 也不碰麥克風。測試用**合成音**（含泛音、刷弦時間差、撥弦衰減）
直接餵進辨識器，所以改動後跑 `npm test` 就知道有沒有壞，不用每次拿起吉他。
**10 支測試**涵蓋和弦辨識、幾何運算、音高偵測、題目產生、樂譜、節奏、指板換算、伴奏樂理，
外加一支「走鐘守衛」擋住兩份程式碼定義不一致。

**⚠️ 也寫清楚它做不到什麼：** 分不出把位與轉位、某些和弦（如 Asus4 與 Dsus2）音級完全相同原理上不可分、
視覺分不出「按下去」與「懸空」。這些不是還沒做，是用這個方法做不到 —— 與其假裝會，不如講明白。

---

### ⭐ [DevLearn — 程式設計學習平台](https://github.com/a0936480350/DevLearn)

232 章教學、8 款遊戲化學習、老師媒合、即時聊天、AI 輔助開發。一個人獨立開發 1 個月。

**🌐 Live Demo:** [devlearn-dotnet.azurewebsites.net](https://devlearn-dotnet.azurewebsites.net/)

**🛠️ 技術棧：** ASP.NET Core 8 MVC · EF Core · PostgreSQL · SignalR · Phaser.js 3

**📊 規模：** 60+ DB tables · 30+ Controllers · 232 章節 · 500+ 題目

---

### 📖 資安工程學習書系（個人著作 · 11 冊 · 93 章）

從網路基礎一路寫到 AI 資安，自己整理的系統化資安工程教材（個人著作，未公開發布）：

1. 電腦與網路基礎
2. Linux 系統基礎與實作
3. Docker 與容器化
4. Kubernetes 與編排
5. Cloud（AWS / Azure / GCP）
6. Cybersecurity 基礎與防禦
7. Wireshark 與封包分析實戰
8. DevSecOps 與自動化安全
9. AI 與資安交集
10. 綜合實戰與職涯
11. VPS 手動部署與 AWS IaC 實戰

---

### 🧩 Xian Knowledge OS — 個人工程作業系統

讓多個開發專案共用標準、決策記錄與經驗，不再各自為政的底層系統（個人使用，架構方法論）：

| 資料夾 | 作用 |
|---|---|
| `standards/` | 命名規範、文件格式、安全基準、寫作風格 |
| `templates/` | 新專案起始樣板 |
| `knowledge/` | 跨專案總覽、依賴關係圖、長期規劃 |
| `decisions/` | 跨專案重大決策紀錄（ADR） |
| `engineering-log/` | 除錯與工程經驗累積 |
| `prompts/` · `mcp/` | AI 協作標準流程 |

核心原則：兩個專案會重複用到的東西放共用層統一維護，需要專案自己事實才能填的內容留在各自專案。

---

### 📂 其他練習作品

較早期的練習專案，技術棧與規模都比較小，列出來記錄學習歷程：

- 🚗 [CarMaintenanceApp](https://github.com/a0936480350/CarMaintenanceApp) — WPF 桌面應用，車輛保養紀錄管理，前後台分離 + Bluetooth 硬體整合
- 🎸 [GuitarSurvey](https://github.com/a0936480350/GuitarSurvey) — ASP.NET Core Razor Pages，吉他課程報名問卷
- 🇯🇵 [JapaneseGames](https://github.com/a0936480350/JapaneseGames) — WinForms 日文學習小遊戲兩款
- [SideProjects](https://github.com/a0936480350/SideProjects) & [practice-work](https://github.com/a0936480350/practice-work) — 日常練習與小型專案集合

---

## 🎓 技術領域

### 後端

- **C#** — OOP、LINQ、async/await、泛型、委派/事件、record、pattern matching
- **ASP.NET Core 8** — MVC、Razor Pages、Web API、SignalR、Middleware、DI 容器、IExceptionHandler、BackgroundService
- **ASP.NET Core Identity** — Cookie auth、ClaimsPrincipalFactory 客製、Multi-tenant 整合、外部 OAuth2（LINE Login 手動串接）
- **EF Core 8** — Code First、Migration、Global Query Filter、SaveChanges Interceptor、複合索引、效能優化、N+1 處理
- **SQL** — Query 優化、Index 設計、Stored Procedure、Window Functions
- **ADO.NET** — 直接操作，理解 ORM 抽象層底下的運作

### Multi-Tenant SaaS 架構（LeadFlow 實戰）

- **ITenantContext** — Claim-based tenant 解析
- **EF Global Query Filter** — 自動為每個 tenant-scoped entity 加 `WHERE TenantId = @ctx`
- **SaveChanges Interceptor** — 寫入時自動蓋章 + 阻擋 anonymous 寫入 + 阻擋 tenant 遷移
- **Identity 表豁免** — 登入流程必須能查 user，跨 tenant 列舉由 service 層 gate
- **Reflection-based filter** — 對所有實作 `ITenantScoped` 的 entity 自動掛載
- **Per-tenant Feature Flag** — (TenantId, FeatureKey) 獨立表 + IMemoryCache + admin UI，支援 Tier B/C 客製化商業模式

### 金流 / 通知 / 整合

- **綠界 ECPay AioCheckOut V5** — SHA256 CheckMacValue 手刻、notify webhook 驗章、訂閱生命週期、到期 worker
- **MailKit + Gmail SMTP** — Outbox pattern、失敗重試、審核狀態追蹤
- **HTML email 範本** — 月報 · 課前提醒 · 家長筆記通知 · 方案到期提醒（inline style 相容各 email 客戶端）
- **LINE Login (manual OAuth2)** — 手動實作 state / nonce / token exchange，家長綁定流程
- **Background services** — EmailOutboxWorker · PreClassReminderWorker · MonthlyReportWorker · PlanExpiryCheckerWorker（24/7 運行）

### 前端 / UI

- **Tailwind CSS + Preline UI** — utility-first，CDN-config 對應 CSS 變數
- **FullCalendar.js 6** — 週/月/日視圖、custom event source、衝堂視覺化
- **JavaScript** — ES6+、Promise、Fetch API、Debounced AJAX validation
- **HTML/CSS** — Flexbox、Grid、RWD（< 480px 小手機優化）、動畫效果
- **遊戲開發** — Phaser.js 3
- **即時通訊** — SignalR Client（WebSocket）

### 桌面開發

- **WPF** — XAML、Data Binding、LiveCharts、前後台分離設計
- **WinForms** — 事件驅動、GDI+、控制項自訂
- **硬體整合** — Bluetooth (32feet.NET)、Serial Port

### 行動開發

- **iOS / Swift** — UIKit、Storyboard、Auto Layout（四約束比例式版面）、AVFoundation 相機管線
- **Apple Vision** — `VNDetectHumanBodyPoseRequest` 骨架偵測、on-device 推論、每點 confidence 處理遮擋
- **AVSpeechSynthesizer** — 語音教練提示
- **My Mac (Designed for iPad)** — Apple Silicon 上直接跑 iOS target（模擬器的 `AVCaptureDevice` 一律回 nil，相機測不了）

### 電腦視覺 / 音訊訊號處理

跨 iOS 與 Web 兩個平台做「即時判斷人做得對不對」的教學工具：

- **姿態偵測** — Apple Vision 19 點（iOS）· MediaPipe HandLandmarker 21 點（Web）
- **幾何判斷** — 三點夾角、向量投影、**除以身體基準正規化**（肩寬 / 掌緣），讓判斷不受相機距離與角度影響
- **單應性變換** — 四點校準求 3×3 投影矩陣，把畫面座標換算成指板座標（含琴衍非線性間距 `1 - 2^(-n/12)`）
- **頻域分析** — FFT → chroma 十二音級能量 → 餘弦相似度比對和弦範本
- **時域分析** — YIN 基頻偵測（累積平均正規化差分壓八度錯誤）＋ 拋物線內插達到 < 1 音分精度
- **音訊合成** — Karplus-Strong 撥弦物理模型、回饋延遲網路殘響、Web Audio 時間軸精準排程（實測抖動 0ms）
- **無硬體測試** — 用合成訊號驗證演算法，不需要樂器或鏡頭就能跑回歸測試

### 架構思維

- **Clean Architecture** — Domain / Application / Infrastructure / Web 嚴格分層
- **SOLID 原則** + **設計模式** — Repository、Strategy、Factory、Observer、Decorator
- **RFC-first** — 重大決策先寫設計文件（`.agents/rfc/` 17 個 RFC）再動手
- **系統設計** — 認證機制（Session/JWT/OAuth/Identity）、快取策略、微服務 vs 單體
- **可觀測性** — Serilog 結構化日誌、RFC 7807 Problem Details、healthcheck endpoints
- **測試策略** — xUnit + WebApplicationFactory 整合測試（InMemory DB + 可切換 ITenantContext）
- **安全性** — SQL Injection 防禦、XSS、CSRF、密碼雜湊、Tenant 跨界保護

### DevOps / Cloud

- **Azure App Service**（Linux .NET 8）+ **Azure Database for PostgreSQL**（Flexible Server）
- **Bicep IaC** — App Service Plan + Web App + Postgres + firewall 一鍵 provisioning
- **GitHub Actions CI/CD** — push to main → restore + build + test + publish + deploy + smoke check
- **Auto-migrate on startup** — 非 Dev 環境部署後自動跑 pending migration
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
| 部署 | Azure App Service · Bicep IaC · Auto-migrate |
| 觀測 | Serilog · Healthcheck endpoints |
| 金流 | 綠界 ECPay AioCheckOut V5 |
| AI 協作 | Claude Code + Codex（兩個 agent 平行協作） |

---

## 📊 作品組合多樣性

| 技術類型 | 代表作 |
|---------|--------|
| Multi-tenant SaaS | LeadFlow.SaaS |
| Web MVC | LeadFlow · DevLearn |
| Web Razor Pages | GuitarSurvey |
| Desktop WPF | CarMaintenanceApp |
| Desktop WinForms | JapaneseGames |
| 即時通訊 | DevLearn (SignalR) |
| 遊戲引擎 | DevLearn (Phaser.js) |
| ADO.NET 直接操作 | CarMaintenanceApp、GuitarSurvey |
| EF Core + 多租戶 | LeadFlow |
| 硬體整合 | CarMaintenanceApp (Bluetooth) |
| 金流整合 | LeadFlow (ECPay V5) |
| OAuth2 手刻 | LeadFlow (LINE Login) |
| CI/CD 自動化 | LeadFlow (Bicep + GH Actions) · DevLearn (GH Actions → Azure) |
| iOS / Swift | ElasticBandCoach (Vision 骨架偵測) |
| 電腦視覺 | ElasticBandCoach (Apple Vision) · Guitar Coach (MediaPipe) |
| 數位訊號處理 | Guitar Coach (FFT / chroma / YIN / Karplus-Strong) |
| 純前端零後端 | Guitar Coach (GitHub Pages) |

---

## 📖 持續學習

透過 DevLearn 平台整理了自己的學習筆記：

- **語法基礎篇**（200+ 章）— C#、SQL、JavaScript、HTML/CSS、Vue、React
- **概念深入篇**（28 章）— 面試常考的觀念：DI、async、REST、系統設計

> 歡迎到 [DevLearn 網站](https://devlearn-dotnet.azurewebsites.net/) 看完整內容！

**2026 年的新方向：** 從純 Web 後端延伸到 **on-device 電腦視覺與訊號處理** ——
用鏡頭與麥克風即時判斷人做得對不對，全部在裝置上運算、不上傳。
`ElasticBandCoach`（iOS/Vision）與 `Guitar Coach`（Web/MediaPipe + Web Audio）是這條線的兩個實作。

做完兩個之後得到一個結論並寫進 ADR：**這類產品的護城河不是偵測技術**（Vision 與 MediaPipe 都免費、
開箱即用），**而是「什麼角度算錯、錯了要講哪一句」** —— 那需要領域教學經驗，不是寫程式能生出來的。

**目前自學中：** RAG（檢索增強生成）、向量資料庫、模型訓練基礎理論 — 還在打底階段，尚未有正式上線的 LLM/RAG 產品。

---

## 📬 聯絡方式

- 💼 GitHub：[@a0936480350](https://github.com/a0936480350)
- 🚀 現役產品：[LeadFlow.SaaS](https://leadflow-mike-tw.azurewebsites.net) · 教務管理中台（音樂 / 才藝 / 補教）
- 🌐 學習平台：[DevLearn](https://devlearn-dotnet.azurewebsites.net/)
- 📱 LINE 官方帳號（DevLearn）：[lin.ee/68vD9ZW](https://lin.ee/68vD9ZW)
- 💬 LINE：`a0936480350`

---

⭐ 如果你覺得 LeadFlow 或 DevLearn 有幫助，歡迎在 GitHub 給個 Star！

<sub>📝 最後更新 2026-08-16 · 新增 ElasticBandCoach（iOS · Apple Vision 骨架偵測）與 Guitar Coach（Web · MediaPipe + Web Audio DSP）· LeadFlow 577 commits / 17 RFC 持續迭代中</sub>
