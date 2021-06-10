# Ping Ping CrowdFunding Website
# 共同檢核點
## 版型檢核點



1. 會檢視 h1~6、ul li、p 語意運用
2. 不要使用 inline style 寫死在 HTML 標籤上
3. 格線系統設計
    * row 裡面第一層只能是 col
    * col 外層只能是 .row
    * 不用寫 `col-12`
4. 單位設計不要出現類似 .width-63、.font-12，以一個單位或等級來設計，例如 `font-xl`、`mb-5`


## 表頭
* logo 請加上 a 連結，通常 logo 都有回首頁的功能
* 一個網站至少會有一個 h1，不會都沒有

## 表單
* label、for 的 focus 沒對應好


### HTML 語意
1. 過度濫用 div，不會利用 ul、li 或 article 與 section
2. 在語意上，有 h2、h4，但卻沒有 h3，在語意規劃上要再留意，這就有點像你寫 word 文件，有副標題，跳過第三標題，確有第四標題
3. 產品價格下了標題標籤
4. 裡面是 p 段落，而非 div
![](https://i.imgur.com/Lb0pjDO.png)
![](https://i.imgur.com/sOnXB0a.png)

### 格線系統
* 不要在 .col 的 HTML 標籤用到 margin 左右推擠

### SCSS 規劃
1. [index.scss](https://github.com/Yiren-Liou/Bootstrap5_crowdfunding/blob/master/assets/scss/_index.scss) 客製化嘗試得不錯，這裡面還可以拆得更好一些，因為有些項目不是只有 index 才有。像是 `.btn-primary` 是每個頁面都有，建議可以多一個像是 `_custom.scss` 來進行擴充，不要都寫在 `index.scss`
2. [GitHub Repo](https://github.com/HaroldZhen/crowdfunding_platform)`Layout` 是共通版型，`index.scss` 應放在 `pages` 資料夾，不建議放在 `Layout`
