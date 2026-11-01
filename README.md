# board-game

## 社會技巧島

我設計的桌遊、社會技巧課程與活動的入口網站，放在 `docs/` 資料夾，用 GitHub Pages 發布。

網址（開啟 GitHub Pages 後）：https://a890823lily-boop.github.io/board-game/

### 第一次開啟 GitHub Pages

1. 到這個 repository 的 **Settings → Pages**。
2. **Source** 選 **Deploy from a branch**。
3. **Branch** 選 `social-skills-island`（或合併後的 `main`），資料夾選 `/docs`，按 **Save**。
4. 等一兩分鐘，上面的網址就能打開。

### 在島上新增東西

島上的內容都寫在 `docs/items.json`。每一項的格式：

```json
{
  "id": "英文代號，不要重複",
  "zone": "board（桌遊港）／lesson（課程村）／practice（練習營）／tool（寶物屋）",
  "title": "名稱",
  "summary": "簡介",
  "audience": "適用對象",
  "skills": ["練習的技巧"],
  "links": [{ "label": "連結名稱", "url": "網址，或放在 docs 裡的網頁路徑" }]
}
```

教材網頁可以放在 `docs/` 底下的資料夾裡（例如 `docs/aquarius/`），連結就寫相對路徑（例如 `aquarius/rules.html`），點了會直接在島上打開。
