# Guide

### 環境

- 放在 Google Cloud 的 `Compue Engine` 上
- 它就是個放在雲端的虛擬機器

### 注意的點

- 沒有連 Google 的其他服務 ( 例如 Cloud SQL 等 )
- 因為所有事都在 machine 裡面做
  - 存放檔案 ( Folder ) 或資料庫 ( SQLite ) 都在本地

### 備份 ( 重要 ! )

- 目前有設定磁碟定時的 [排程快照](https://cloud.google.com/compute/docs/disks/create-snapshots?hl=zh-tw)
