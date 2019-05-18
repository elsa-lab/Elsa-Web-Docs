# Datebase

1. 使用 `SQLite` 資料庫
2. 若要進入 management page，只能是老師的身分
   - 把 `user_profile` table 中對應的 studentType 加上 root_user_types
   - root_user_types 請參考 frontend/src/settings.js