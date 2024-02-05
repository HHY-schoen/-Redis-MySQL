使用 python 實作登入模擬系統：使用者輸入「帳號」，網站收到帳號去尋找對應的「密碼」。
- 嘗試從 redis 拿取密碼 Ｘ。如果找到密碼就回傳值
- 如果拿不到密碼，就去 mysql 裡面找。如果找到密碼 X 回傳後，寫一筆到 redis 中
- 若 mysql 也找不到密碼，就寫一筆到 mysql 中、並同時也寫一筆到 redis 中，最後回傳密碼。

## Redis
Redis 是一個 in-memory 的 key-value database，常被用在需要快取（Cache）一些資料的場合，可以減輕資料庫的負擔，同時也加快響應速度。
