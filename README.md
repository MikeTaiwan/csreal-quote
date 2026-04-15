# CS Real 報價單系統

## 本機開發

```bash
npm install
npm run dev
```

## 部署到 GitHub Pages

### 第一次設定

1. 在 GitHub 建立新 repo，名稱建議：`csreal-quote`
2. 確認 `vite.config.js` 裡的 `base` 與 repo 名稱一致：
   ```js
   base: '/csreal-quote/',
   ```
3. 推上 GitHub：
   ```bash
   git init
   git add .
   git commit -m "init"
   git branch -M main
   git remote add origin https://github.com/你的帳號/csreal-quote.git
   git push -u origin main
   ```
4. 到 GitHub repo → Settings → Pages → Source 選 **gh-pages** branch

### 之後更新

每次 push 到 main，GitHub Actions 會自動重新建置並部署，約 1 分鐘生效。

```bash
git add .
git commit -m "更新品項價格"
git push
```

## 網址

部署完成後網址為：
```
https://你的帳號.github.io/csreal-quote/
```
