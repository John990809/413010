# 🎵 Cyber Beat - 霓虹節奏遊戲 (Cyber Beat Rhythm Game)

![Cyber Beat Preview](https://img.shields.io/badge/Game-Cyber%20Beat-cyan?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

一款充滿賽博朋克霓虹風格的網頁版 4 軌道（4 Lanes）節奏動作遊戲！無須安裝任何額外外掛，開啟瀏覽器即可體驗節奏感十足的音樂遊戲。

---

## 1. 霓虹節奏遊戲
* **中文名稱**：Cyber Beat - 霓虹節奏遊戲
* **英文名稱**：Cyber Beat Rhythm Game

---

## 2. 遊戲玩法
* **基本規則**：音符會隨著音樂節奏從上方往下掉落至底部的「判定線」。當音符抵達判定線的瞬間，按下對應的按鍵即可得分並保持連擊（Combo）。
* **判定機制**：根據按鍵的時間精準度分為 `PERFECT`、`GREAT`、`GOOD` 與 `MISS`。
* **生命值機制**：精準擊中音符可恢復生命值（LIFE）；若漏抓音符（MISS）則會扣除生命值。生命值歸零時遊戲失敗（STAGE FAILED）。

---

## 3. 使用的 AI 提示詞 (AI Prompts)

本專案使用以下提示詞引導 AI 生成遊戲核心架構與視覺效果：

> *"請使用 Web Audio API 與 Canvas 打造一款 4 軌道 (A, S, K, L) 節奏遊戲。包含多首動態合成音效歌曲、連擊系統、判定打擊粒子特效、下落速度調節、生命值血條以及完整的遊戲結果統計。使用單一 HTML 檔案包含所有 JS/CSS，並以 Tailwind CSS 做美化。"*

---

## 4. 已完成的功能

- 🔊 **Web Audio API 原生音效合成引擎**：無需載入外部 MP3 檔，由瀏覽器即時生成 8-bit / Synthwave 節奏音樂與打擊音效。
- 🎯 **動態 Canvas 渲染系統**：包含霓虹發光軌道、判定線閃爍動畫與精準的擊中粒子爆炸特效（Particle System）。
- 📊 **完整結算與評級**：即時計算 Accuracy（準確率）、Max Combo（最高連擊），並在通關後給予 S / A / B / C / F 等級判定。
- ⚡ **自訂下落速度**：支援 0.6x 至 2.0x 的音符流速調節，適應不同玩家的反應習慣。
- 📱 **響應式與觸控支援**：除了鍵盤操作外，畫面下方提供觸控按鈕，支援手機與平板體驗。
- 🎵 **多曲目選擇**：內建不同 BPM 與難度（EASY / MEDIUM / HARD）的挑戰歌曲。

---

## 5. 操作方式 (Controls)

| 軌道 (Lane) | 按鍵 (Key) | 說明 |
| :--- | :---: | :--- |
| **Lane 1** (最左) | <kbd>A</kbd> | 點擊第 1 軌音符 |
| **Lane 2** (中左) | <kbd>S</kbd> | 點擊第 2 軌音符 |
| **Lane 3** (中右) | <kbd>K</kbd> | 點擊第 3 軌音符 |
| **Lane 4** (最右) | <kbd>L</kbd> | 點擊第 4 軌音符 |

* 📱 **行動裝置/觸控螢幕**：直接點擊畫面下方對應的 **A**、**S**、**K**、**L** 虛擬按鈕即可遊玩。

---

## 6. 作品連結 (Project Link)

* **核心入口檔案**：[`index.html`](./index.html)
* **快速預覽**：直接使用瀏覽器雙擊開啟 `index.html`，或搭配 VS Code 的 Live Server 套件開啟即可直接遊玩。

---

## 🛠️ 技術棧 (Tech Stack)

* **Frontend**: HTML5, JavaScript (ES6+), Tailwind CSS (CDN)
* **Graphics**: HTML5 `<canvas>` API
* **Audio**: Web Audio API (AudioContext)
* **Icons & Fonts**: Font Awesome, Google Fonts (Orbitron / Noto Sans TC)
