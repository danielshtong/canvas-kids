# canvas-kids

小學（小四至小六）AI 課程示範網頁。GitHub Pages 由 `main` 分支根目錄發佈。

## 第2節 Gemini Canvas 自製溫習材料

- `index.html`：學生用提示詞卡（由 `build.py` + `template.html` 生成，改提示詞請改 `build.py` 再執行 `python3 build.py`）
- `demo1/`：示範例子 1，食物英文生字閃卡
- `demo2/`：示範例子 2，食物生字配對遊戲
- `qr/`、`shots/`：QR code 同截圖

生字表喺每個示範檔案最頂嘅 `WORDS` array。

## 第3節 學生自製溫習閃卡

- `maker/`：學生自己寫正面、背面，反轉預覽，整一副最多 10 張嘅閃卡，做負責任 AI 八點檢查，再列印或者下載。純靜態 HTML／CSS／JS，卡片儲存喺瀏覽器 localStorage。
- 公開網址（投影片 QR code 用呢個）：https://danielshtong.github.io/canvas-kids/maker/
