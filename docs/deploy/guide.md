# Guide

### 環境

- 放在 Google Cloud 的 `Compue Engine` 上 ( 就是放在雲端的虛擬機器 )
- 只有 `Elsa Web` 專案底下的才是 Web 用的，不要亂刪到別人的 !!
- 目前是前後端各一個 machine
  - 可以討論未來是否要合併 ? https ?
- 後端的 machine 有給好一點，因為處理 pdf to image 需要

### 更新

-  machine 裡的 code 是用 git 來更新 ( local 寫完 push，remote 再 pull )
-  前端
   -  把 build 完的資料夾移到 `Elsa-Lab-Static` 中 ( machine 裡放的是這個 project，而不是 frontend )
- 後端
  - .gitignore 裡有 `course_data` / `publications_file` / `db.sqlite3`
  - 所以改了後端 code，到 machine 裡 pull 下來，不會汙染到儲存資料 ( 就是上面這三個 )

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
