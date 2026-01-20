Colonial Comedy Interactive ESL Learner

這是一個為台灣 ESL 學生設計的互動式學習網頁，內容基於 Trevor Noah 的脫口秀片段，旨在透過幽默的語境幫助學生掌握高階英語詞彙與文化背景。

專案亮點

互動單字卡：11 個核心單字，具備大字體設計與翻面翻譯功能。

地道片語解析：深入解析諷刺幽默中常用的固定搭配。

文化深度解讀：針對多神教與一神教、殖民視角轉換等文化落差提供雙語說明。

解鎖式晉級挑戰：包含 19 題 Level 1 & Level 2 測驗，學生必須答對正確答案才能解鎖背面的解析。

成就獎勵系統：完成每一等級的所有挑戰後，會彈出精美的讚美勳章，提升學習動機。

舒適配色設計：採用米棕色 (Warm Oatmeal) 與淡綠色 (Sage Green) 的配色方案。

如何在本地執行

本專案使用 React + Tailwind CSS 開發。您可以透過以下步驟在您的電腦上運行：

建立 React 專案 (建議使用 Vite):

npm create vite@latest my-esl-app -- --template react
cd my-esl-app


安裝必要套件:

npm install lucide-react
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p


配置 Tailwind CSS:
在 tailwind.config.js 中加入以下路徑：

/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}


替換程式碼:
將本專案的 App.jsx 內容完全覆蓋您專案中的 src/App.jsx。

執行專案:

npm run dev


技術棧

React (Hooks: useState, useEffect)

Tailwind CSS (用於響應式佈局與配色)

Lucide React (圖示庫)

CSS Perspective (用於 3D 翻牌效果)

本內容僅供教學研究使用，脫口秀文本版權屬於原創作者 Trevor Noah。
