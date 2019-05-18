# App

### home
  - about
    - lab 介紹 ( 教授 & 學生 )
  - user
      - 未登入
        - Sign In
        - Sign Up
      - 已登入
        - Account

### courses
  - course ( 課程名稱 ) → content ( 每年開設的課程 ) → lecture ( 課程中的每一堂課 )
  - file ( 屬於 lecture )
  - comment ( 屬於 file， 並記錄頁碼 )

### publications
  - arXiv
  - PDF

### projects 
  - 純前端 ( 同個 template )
  - 根據 project 不同去微調 CSS

### news
  - 點進去有詳細內文
  - 從後端拿到 Rich Text 形式文字

### management
若要進入此頁面，只能是老師的身分
> 把 `user_profile` table 中對應的 studentType 加上 root_user_types
>
> `root_user_types` 請參考 settings.js

  - users
  - courses
  - publications
  - news
    - 使用 Rich Text 編輯器