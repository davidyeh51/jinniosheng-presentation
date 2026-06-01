# 進金生能源服務 — 公司簡報

線上展示版本，由 [GitHub Pages](https://pages.github.com/) 提供服務。

## 線上瀏覽

> 啟用 GitHub Pages 後，網址為：  
> **`https://<your-username>.github.io/<repo-name>/`**

## 操作說明

| 操作 | 功能 |
|------|------|
| `→` / `Space` / 點右半部 | 下一張 |
| `←` / 點左半部 | 上一張 |
| `F` | 全螢幕（業務展示模式） |
| `T` | 縮圖總覽 |
| `Home` / `End` | 跳到第一 / 最後一張 |
| 手機左右滑動 | 換頁 |

## 發佈步驟

```bash
# 1. 建立 GitHub 倉庫（在 GitHub 網站新增一個 public repo）

# 2. 初始化並推送
git init
git add .
git commit -m "feat: 公司簡報網頁版"
git branch -M main
git remote add origin https://github.com/<username>/<repo>.git
git push -u origin main

# 3. 在 GitHub 倉庫設定 → Pages → Source 選 main / (root)
# 數分鐘後即可透過 https://<username>.github.io/<repo>/ 瀏覽
```

## 更新投影片

1. 將新的 `.pptx` 重新匯出為 PNG，覆蓋 `slides/` 資料夾內的檔案
2. `git add slides/ && git commit -m "update: 更新投影片" && git push`
3. GitHub Pages 約 1–2 分鐘後自動更新

## 檔案結構

```
├── index.html       # 簡報播放器（單檔，無外部依賴）
├── slides/
│   ├── slide-01.png ~ slide-22.png
└── README.md
```
