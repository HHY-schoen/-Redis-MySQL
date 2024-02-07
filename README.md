使用 python 實作登入模擬系統：使用者輸入「帳號」，網站收到帳號去尋找對應的「密碼」。
- 嘗試從 redis 拿取密碼 Ｘ。如果找到密碼就回傳值
- 如果拿不到密碼，就去 mysql 裡面找。如果找到密碼 X 回傳後，寫一筆到 redis 中
- 若 mysql 也找不到密碼，就寫一筆到 mysql 中、並同時也寫一筆到 redis 中，最後回傳密碼。

## Redis
Redis ( Remote Dictionary Server ) 是一個 in-memory 基於內存的 key-value database，常被用在需要資料庫緩存、快取（Cache）資料和消息隊列的場合，可以減輕資料庫的負擔，同時也加快響應速度。

- docker pull redis



------------------------
refer
- https://medium.com/%E7%A8%8B%E5%BC%8F%E4%B9%BE%E8%B2%A8/python-redis-v-s-mysql-%E6%9F%A5%E8%A9%A2%E5%AF%A6%E4%BD%9C-9f0cc0d9b32b
- https://github.com/pcchencode/python-redis/blob/master/redis.ipynb
