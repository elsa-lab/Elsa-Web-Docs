# Guide

### 環境

- 放在 Google Cloud 的 `Compue Engine` 上 ( 就是放在雲端的虛擬機器 )
- 只有 `Elsa Web` 專案底下的才是 Web 用的，不要亂刪到別人的 !!
- 目前是前後端各一個 machine
  - 使用 [serve](https://github.com/zeit/serve) 部署前端靜態檔案
  - 討論一下未來是否要合併 ? https ? 可以研究一下
- 後端的 machine 有給好一點，因為處理 pdf to image 需要

### 網址
> 網域的部分，要等系計中幫忙用，但他們現在缺人
> 
> 所以先暫時用底下的網址

- 前端 : http://35.229.221.5:8080/
- 後端 : http://35.201.173.113:8080/

### 注意的點

- 沒有連 Google 的其他服務 ( 例如 Cloud SQL 等 )
- 因為所有事都在 machine 裡面做
  - 存放檔案 ( folder ) 或資料庫 ( SQLite ) 都在本地

### 備份 ( 重要 ! )

- 目前有設定磁碟定時的 [排程快照](https://cloud.google.com/compute/docs/disks/create-snapshots?hl=zh-tw)
