# LiMA 永續選品型錄

簡約高端風格的永續選品型錄網站，適合直接部署至 GitHub Pages。

## 頁面結構

| 檔案 | 說明 |
|------|------|
| `index.html` | 首頁（品牌介紹、精選選品、品牌價值） |
| `catalog.html` | 選品型錄（分類篩選、12+ 商品列表） |
| `product.html` | 單品詳情（圖片切換、規格、認證、評價） |
| `about.html` | 品牌理念（故事時間軸、選品標準、團隊） |
| `contact.html` | 聯絡我們（表單、FAQ） |
| `style.css` | 全站共用樣式 |
| `main.js` | 全站共用 JS（導覽、滾動動畫） |

## 部署到 GitHub Pages

1. 在 GitHub 建立新 Repository，名稱建議：`lima-catalog`
2. 將所有檔案上傳至 Repository 根目錄
3. 前往 Settings → Pages → Source 選擇 `main` branch / `root`
4. 稍待幾分鐘，網站即可透過 `https://<你的帳號>.github.io/lima-catalog/` 訪問

## 自訂內容

### 替換圖片
目前所有商品圖片為漸層色塊佔位。替換方式：
- 將圖片放入 `images/` 資料夾
- 將 `<div class="img-placeholder ...">` 替換為 `<img src="images/你的圖片.jpg" alt="..." />`

### 修改選品資料
在 `catalog.html` 中每個 `.product-card` 區塊可自由修改：
- 商品名稱、描述、價格
- 分類標籤（`data-category` 屬性需對應篩選按鈕）

### 修改品牌資訊
- 色票變數集中於 `style.css` 的 `:root` 區塊
- 頁尾聯絡資訊、社群連結在各頁面 `<footer>` 內

## 設計規格

- **主色調**：自然鼠尾草綠 `#7A8C6E` / 深林綠 `#4A5E3A`
- **字型**：Cormorant Garamond（標題）· DM Sans（內文）· Noto Serif TC（中文）
- **風格**：簡約高端，白底精緻排版，留白充足
- **響應式**：支援桌機、平板、手機三種斷點
