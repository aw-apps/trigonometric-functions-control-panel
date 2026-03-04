# 三角函數互動控制面板

這是從 `doggy8088/trigonometric-functions` 延伸的客製化版本，目標是加入更易用的互動控制面板，讓使用者可直接調整角度與播放速度，並即時查看 `sin/cos/tan` 數值。

## 專案目標

- 提供可視化的單位圓與波形動畫
- 新增互動控制面板（角度、速度、播放狀態）
- 同步顯示三角函數數值，提升教學與學習效率

## 技術堆疊

- HTML5
- CSS3
- JavaScript (ES6+)
- Three.js（沿用原始專案）

## 本地執行

```bash
python3 -m http.server 8080
# 開啟 http://localhost:8080
```

## 手動驗證（Validation）

1. 開啟頁面後連續操作至少 2 分鐘：拖曳或輸入角度、切換速度、播放/暫停交替。
2. 確認控制面板角度、畫面中角度位置與 `sin/cos/tan` 即時數值維持同步。
3. 重新整理頁面後，再次確認上述核心互動都可正常運作。

## 部署（GitHub Pages）

建議使用 GitHub Pages（`main` 分支 root），部署前請確認：

- [ ] 所有變更已推送到 `main`
- [ ] Repository Settings → Pages 已設定為 `Deploy from a branch`
- [ ] Branch 選擇 `main`，資料夾選擇 `/ (root)`
- [ ] 重新開啟 GitHub Pages 網址，並完成「手動驗證（Validation）」流程
