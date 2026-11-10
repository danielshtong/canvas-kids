# canvas-kids

小學（小四至小六）AI 課程示範網頁。GitHub Pages 由 `main` 分支根目錄發佈。

## 第2節 Gemini Canvas 自製溫習材料

- `index.html`：學生用提示詞卡（由 `build.py` + `template.html` 生成，改提示詞請改 `build.py` 再執行 `python3 build.py`）
- `demo1/`：示範例子 1，食物英文生字閃卡
- `demo2/`：示範例子 2，食物生字配對遊戲
- `qr/`、`shots/`：QR code 同截圖

生字表喺每個示範檔案最頂嘅 `WORDS` array。

課程主頁（`index.html`）有連結去第3節、第4節同第5節。

## 第3節 學生自製溫習閃卡

- `maker/`：學生自己寫正面、背面，反轉預覽，整一副最多 10 張嘅閃卡，做負責任 AI 八點檢查，再列印或者下載。純靜態 HTML／CSS／JS，卡片儲存喺瀏覽器 localStorage。
- 公開網址（投影片 QR code 用呢個）：https://danielshtong.github.io/canvas-kids/maker/

## 第4節 AI 學習任務包

- `mission/`：總任務。預設主題係「幫同學複習一個課題」。學生揀課題（交通安全、環保、校園禮儀或者自訂），完成三個通關步驟：用 AI 做插圖／海報、做複習閃卡（連去 `maker/`，亦可試 `demo1/`）、同負責任 AI 八點自評。私隱、真實、負責三項剔咗會顯示「可以分享」。再寫作品筆記同三句總結，睇進度，完成就慶祝。可以列印任務包，或者下載文字／JSON。純靜態，冇登入，資料喺瀏覽器 localStorage（鍵名 `canvas-kids-mission-v1`）。
- 公開網址（投影片 QR code 用呢個）：https://danielshtong.github.io/canvas-kids/mission/

## 第5節 提示小老師

- `hint/`：社區任務課。學生設計「提示小老師」提示包（題目、由淺入深嘅提示、可選引導問題、收起嘅標準答案），做同第3節一樣嘅負責任 AI 八點檢查，複製 Gemini Gem 提示詞，或者用分享連結俾同學互測。互測只會一個一個揭提示；睇晒提示再自己確認「自我核對」，先至見到標準答案。純靜態，資料喺瀏覽器 localStorage（鍵名 `canvas-kids-hint-v1`），分享連結用網址 hash，冇伺服器。
- 公開網址（投影片 QR code 用呢個）：https://danielshtong.github.io/canvas-kids/hint/
