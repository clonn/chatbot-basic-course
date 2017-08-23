\#\# 執行 Messenger　範例



---



\#\# 接下來需要準備

1. 粉絲粉權杖的 Token

2. 認證用 Token



---



\#\# 一、取得粉絲團權杖

!\[\]\(https://i.imgur.com/ixgLUD0.png\)



---



\#\# 跳出 FB 身份登入確認

!\[\]\(https://i.imgur.com/e6JXsGK.png\)



---



\#\# 確認後會要求授權

!\[\]\(https://i.imgur.com/NkuNB6s.png\)



---



\#\# 權杖就會產生出來

!\[\]\(https://i.imgur.com/o0elNYl.png\)



---



\#\# 啟動 ngrok

\`\`\`shell

ngrok http 3000

\`\`\`

!\[\]\(https://i.imgur.com/otQbV2m.png\)



---



\#\# 下載範例程式

\`\`\`shell

git clone https://github.com/urmatbay/fb-chatbot.git

\`\`\`



---



\#\# Terminal 切換到 Sample 資料夾

\`\`\`shell

cd fb-chatbot

\`\`\`



---



\#\# 安裝 Node Modules \(擇一\)

\`\`\`shell

npm install / yarn install

\`\`\`

!\[\]\(https://i.imgur.com/FNkilDF.png\)



---



\#\# 設定相關資訊

\#\#\#\# 方式一

\`\`\`shell

export PAGE\_ACCESS\_TOKEN={粉絲團權杖 Token}

export VERIFY\_TOKEN={Webhook 驗證權杖}

\`\`\`



\#\#\#\# 方式二

\`\`\`js

第 22 行 process.env.VERIFY\_TOKEN 改為 "{Webhook 驗證權杖}"

第 187 行 process.env.PAGE\_ACCESS\_TOKEN 改為 "{粉絲團權杖 Token}"



\`\`\`



---



\#\# 起啟 Webhook Server

\`\`\`shell

npm start

\`\`\`



---



\#\# 設定 Webhook

\#\#\#\# ngrok https 的連結和 VERIFY\_TOKEN

!\[\]\(https://i.imgur.com/9CnvfZS.png\)



---



\#\# 設定 FB Messenger Webhook

!\[\]\(https://i.imgur.com/qF62JMJ.png\)



---



\#\# Webhook 設定成功

!\[\]\(https://i.imgur.com/1TAVnuc.png\)



---



\#\# 選擇訂閱粉絲團

!\[\]\(https://i.imgur.com/PPF6Xgt.png\)



---



\# 測試 ChatBot



---



\#\# 到粉絲團開啟 Messenger

!\[\]\(https://i.imgur.com/UNYe6sZ.png\)



---



\#\# 選擇「發送訊息」

!\[\]\(https://i.imgur.com/IPjXlDB.png\)



---



\#\# 來測試 Messenger

!\[\]\(https://i.imgur.com/mJlPWuQ.png\)



---



\#\# 說什麼 Chatbot 回什麼

!\[\]\(https://i.imgur.com/ZWDnxkO.png\)



---

