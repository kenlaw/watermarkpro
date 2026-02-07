iClass WatermarkPro (v1.26020309)
專業級防 AI 浮水印與 PDF 內容鎖定工具

這是一個基於瀏覽器的單文件 (Single-file) 工具，無需伺服器，專為保護教學資源、機密文件與圖片設計。所有處理皆在本地端 (Client-side) 完成，確保資料絕對安全。

【 專 案 簡 介 】

iClass WatermarkPro 整合了 React、Tailwind CSS 與強大的 PDF 處理核心 (pdf-lib, pdf.js)。只要下載一個 .html 檔案，即可在任何現代瀏覽器中運行。它特別針對「防止 AI 去除浮水印」進行了優化，並支援將 PDF 文字轉為外框 (Rasterization)，徹底防止內容被選取或複製。

【 核 心 功 能 】

[1] 批量處理系統 (Batch Processing)
支援拖放上傳多個 PDF 或圖片 (PNG/JPG)。
單檔直接下載，多檔自動打包為 ZIP。
支援 PDF 頁數上限提示更新至 500 頁。

[2] 強效防護技術 (Anti-AI & Security)
雜訊干擾 (Noise)：添加隨機噪點，干擾 AI 修復算法。
隨機化 (Randomization)：微調角度與位置，打破規律性。
漸層填充 (Gradient)：使用非純色填充，增加去除難度。
[Beta] 文字轉外框 / 內容光柵化：將 PDF 強制轉為高解析度圖片，徹底鎖定文字，防止選取或複製。

[3] 智慧畫質管理
超高清 (Ultra)：360 DPI (100% 品質)，轉外框專用，最接近向量原檔。
高畫質 (High)：216 DPI (95% 品質)，適合一般印刷。
普通 / 快速：適合螢幕瀏覽與快速傳輸。

[4] 一鍵快速設定 (Quick Presets)
一般保密：標準設定 (透明度 20%)。
離線課本：高密度、低透明度 (10%)。
僅轉外框：無浮水印，僅執行 PDF 鎖定功能。

[5] 真實預覽技術
整合 pdf.js，直接渲染 PDF 首頁內容，所見即所得 (WYSIWYG)。

【 如 何 使 用 】

STEP 1: 下載本 Repo 中的 watermark_pro.html 檔案。
STEP 2: 直接使用 Chrome、Edge 或 Safari 瀏覽器打開該檔案。
STEP 3: 拖放文件，調整設定，點擊下載即可。

【 技 術 棧 】

核心框架：React 18 (經由 Babel Standalone 編譯)
樣式設計：Tailwind CSS (CDN)
PDF 核心：pdf-lib (生成) / pdf.js (渲染)
檔案壓縮：JSZip
系統架構：Single-file HTML (無後端)

【 版 本 紀 錄 】

v1.26020309
新增「超高清 (Ultra)」畫質選項 (Scale 5.0)。
優化「僅轉外框」模式，預設使用 Ultra 畫質以解決文字模糊問題。

v1.26020306
重寫繪圖引擎，採用圖層分離技術，解決圖片背景變黑與雜訊問題。

v1.26020305
加入 PDF 光柵化核心，實現真正的「文字轉外框」防複製功能。

=====================================================
(c) iClass | 專為內部或授權用戶使用