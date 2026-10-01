# N5 Study Tools

自學日文 N5 檢定用的練習小工具，純靜態網頁，不需要安裝任何東西，不需要後端。

## 工具

- **[五十音道場](gojuon-dojo/index.html)** — 平假名反應速度測驗（清音／濁音半濁音／拗音），記錄反應時間，自動標出弱點字。
- **[単語道場](tango-dojo/index.html)** — N5 核心單字連續 flashcard，先看假名讀音自己回想意思，點開才看漢字跟中文。

## 怎麼用

直接用瀏覽器打開對應的 `index.html` 即可，或是本機起一個簡單的靜態伺服器：

```bash
python3 -m http.server 8000
```

然後瀏覽 `http://localhost:8000/gojuon-dojo/` 或 `http://localhost:8000/tango-dojo/`。

練習進度（弱點字記錄）存在瀏覽器的 `localStorage`，只存在同一個瀏覽器裡，換瀏覽器或清除網站資料會重置。

## 開發說明

給接手開發的細節寫在 [CLAUDE.md](CLAUDE.md)，包含設計決策、視覺系統、建議的後續方向。
