# 數位導覽 語言自動切換網頁 說明

## 這是什麼

館內 18 個 QR Code 不變，只改 Lihi 短網址的目標。遊客掃描後先到這個網頁，網頁讀手機的語言設定，自動打開同一集的對應語言版本：

- 中文（繁體、簡體）→ 中文節目
- 日文 → 日文節目
- 韓文 → 韓文節目
- 其他語言 → 英文節目

畫面會停留 3 秒再自動跳轉，這段時間可以用畫面上的四個語言按鈕手動切換。遊客手動選過一次後，網頁會記住，之後掃其他展示物都直接用那個語言。

網址後面加 `&stay=1` 可以停在選語言的畫面，不自動跳轉，方便測試。

## 檔案

- `index.html`：網頁本身，放到 GitHub Pages。四語各 18 集的 SoundOn 單集連結都寫在裡面。

## Lihi 要改的 18 個短網址

| 集數 | 短網址（QR Code 內容） | 展示物 | 新的目標網址 |
|---|---|---|---|
| 1 | yst1880.com/teaculturehouseintro | 遊山茶訪茶文化館-引言 | https://chenxandy.github.io/audio-guide/?ep=1 |
| 2 | yst1880.com/teaplantation | 茶產區介紹 | https://chenxandy.github.io/audio-guide/?ep=2 |
| 3 | yst1880.com/teastock | 茶文物介紹-青果合作社股票 | https://chenxandy.github.io/audio-guide/?ep=3 |
| 4 | yst1880.com/teapackage | 茶文物介紹-茶葉包裝發展過程 | https://chenxandy.github.io/audio-guide/?ep=4 |
| 5 | yst1880.com/teaaward | 茶文物介紹-茶獎狀、吳振鐸場長 | https://chenxandy.github.io/audio-guide/?ep=5 |
| 6 | yst1880.com/tearing | 茶文物介紹-茶剪、祖母的戒指、炒茶版 | https://chenxandy.github.io/audio-guide/?ep=6 |
| 7 | yst1880.com/teawithering | 茶葉製造-萎凋 | https://chenxandy.github.io/audio-guide/?ep=7 |
| 8 | yst1880.com/teapanfiring | 茶葉製造-炒菁 | https://chenxandy.github.io/audio-guide/?ep=8 |
| 9 | yst1880.com/tearolling | 茶葉製造-揉捻 | https://chenxandy.github.io/audio-guide/?ep=9 |
| 10 | yst1880.com/tearoasted | 茶葉製造-烘焙 | https://chenxandy.github.io/audio-guide/?ep=10 |
| 11 | yst1880.com/teakneading | 茶文物介紹-採茶工具、團揉工具 | https://chenxandy.github.io/audio-guide/?ep=11 |
| 12 | yst1880.com/uniquetea | 獨特的遊山茶訪烏龍茶 | https://chenxandy.github.io/audio-guide/?ep=12 |
| 13 | yst1880.com/teatasting | 茶葉品鑑 | https://chenxandy.github.io/audio-guide/?ep=13 |
| 14 | yst1880.com/teainspection | 茶檢驗室 | https://chenxandy.github.io/audio-guide/?ep=14 |
| 15 | yst1880.com/teaceromony | 茶禮介紹-林易山老師 | https://chenxandy.github.io/audio-guide/?ep=15 |
| 16 | yst1880.com/teaconfucius | 茶禮介紹-儒家茶禮 | https://chenxandy.github.io/audio-guide/?ep=16 |
| 17 | yst1880.com/teafourseason | 茶禮介紹-四序茶會 | https://chenxandy.github.io/audio-guide/?ep=17 |
| 18 | yst1880.com/teabeauty | 茶禮介紹-東方美人頌 | https://chenxandy.github.io/audio-guide/?ep=18 |

網頁網址：https://chenxandy.github.io/audio-guide/

## 目前狀態（2026.11.10）

- 網頁已上線：https://chenxandy.github.io/audio-guide/
- Lihi 的 18 個短網址都已改指到上表的新目標網址。
- 原本的目標是 Apple Podcasts 上《凍茶力》的舊版數位導覽單集（網址後面帶 utm_source=teaculturehouse&utm_medium=qrcodescan）。如果要改回去，到 Lihi 把目標換回《凍茶力》對應集數即可。

## 之後要更新時

- 節目或單集重新上傳、SoundOn 單集網址變了：改 `index.html` 裡的單集代碼。
- 新增語言：在 `index.html` 加一組節目代碼和 18 集代碼。

## 修訂紀錄

| 日期 | 版本 | 內容 | 修改者 |
|---|---|---|---|
| 2026.11.10 | 1 | 初版：建立語言自動切換網頁與 Lihi 對照表 | Claude |
| 2026.11.10 | 2 | 填入 GitHub Pages 網頁網址 | Claude |
| 2026.11.10 | 3 | Lihi 18 個短網址改指到語言切換網頁，記錄原本目標 | Claude |
| 2026.11.10 | 4 | 自動跳轉前的停留時間改為 3 秒 | Claude |
| 2026.11.10 | 5 | 提示文字改為四種語言並列 | Claude |
