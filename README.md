# 依洛嘉面膜保養官方旗艦店

> 平價保養品第一品牌｜SINCE 2004

依洛嘉國際實業有限公司的官方網站，提供客戶瀏覽商品資訊、促銷訊息與線上購物入口。
採用電商型首頁、森林系配色（自然清新），並支援 RWD（手機、平板、桌機）。

純 **HTML + CSS** 製作，沒有使用 JavaScript，也不需要建置工具。

## 頁面

| 檔案 | 說明 |
|---|---|
| `index.html` | 首頁：輪播圖、快捷入口、最新商品、依膚質選購、品牌故事、社群連結 |
| `contact.html` | 聯絡我們：線上留言表單、聯絡資訊、Google 地圖 |
| `downloads.html` | 面膜相關檔案下載：`files/原料/` 內的 MSDS／COA 文件 |
| `cloud-downloads.html` | 面膜原料雲端相關檔案下載：連到 Google 雲端硬碟的同一批文件 |

## 專案結構

```
.
├── index.html
├── contact.html
├── downloads.html
├── cloud-downloads.html
├── style.css              # 全站樣式（配色、RWD、互動效果）
├── images/                # 依膚質選購區的 SVG 插圖
├── files/原料/            # 可下載的 PDF 文件
├── elg-menu.md            # 資料來源：選單
├── elg-latest-products.md # 資料來源：最新商品
├── elg-carousel.md        # 資料來源：輪播圖
├── elg-social.md          # 資料來源：社群連結
└── .claude/               # 本機預覽用設定
```

## 功能特色

- **森林系配色**：深森林綠為主色，暖陶土色作促銷與購買按鈕的點綴，米白底色。
- **RWD**：手機（小於 768px）漢堡選單、商品每排 2 張；平板每排 3 張；桌機每排 5 張。
- **主選單**：「保養」為兩欄大型選單，其餘為下拉選單，手機版可逐層展開。
- **輪播圖**：純 CSS 自動輪播，滑鼠移上去暫停。
- **互動效果**：按鈕滑過變色、捲動時區塊淡入、選單平滑捲動。瀏覽器設為「減少動態效果」時會自動關閉。
- **Icon 圖示**：Font Awesome 6 免費版（透過 cdnjs 載入）。

## 本機預覽

網站是靜態檔案，用瀏覽器直接開啟 `index.html` 即可。若需要透過本機伺服器預覽（Windows PowerShell）：

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File .claude/serve.ps1
```

然後開啟 <http://localhost:8090/>。

## 注意事項

- **購物車**：商品的「加入購物車」目前只是連到商品頁，沒有真正的購物車功能。購物車與結帳需要後端才能實作。
- **留言表單**：使用 `mailto:`，送出時會開啟訪客的電子郵件程式，並不是直接由網站寄出。
- **外部圖片**：Logo、輪播圖、商品圖與社群圖示直接引用舊官網的圖片伺服器（`image-cdn-flare.qdm.cloud`）。若舊站關閉或更換圖片，這些圖會失效，建議之後下載到 `images/` 改用本機路徑。
- **雲端下載頁**：Google 雲端硬碟的連結需將共用權限設為「知道連結的人可檢視」，訪客才能開啟。
- **檔案名稱**：下載頁顯示的名稱已轉為繁體，實際檔案名稱仍是簡體。
- 資料來源（選單、商品、輪播圖、社群）整理自舊官網 <https://www.elg.com.tw/>，內容以官方為準。

## 公司資訊

依洛嘉國際實業有限公司

- 統一編號：53796463
- 營業時間：周一至周五上午 09：00 -下午 05：00
- 服務地址：台南市佳里區佳興里宅興二街600號
- 客服電話：(06)7266551
- 傳真電話：(06)7263656
- 官方 LINE ID：@def6392t
- 官方 FB：E.L.G依洛嘉
- 官方 IG：e.l.g_mask_taiwan
- 官方 YouTube：E.L.G依洛嘉國際
- E-mail：sunnyelg1118@gmail.com

SINCE 2004 © by ELG Taiwan
