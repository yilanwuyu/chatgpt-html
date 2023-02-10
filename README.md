# Chat-GPT
Ai-Chat

Update the key on line 47 of the index.html file

online: https://chatgpt.sbaliyun.com/

部署 ChatGPT-Html

依赖环境初始化完成后，我们马不停蹄，立刻将该项目克隆至服务器内：

git clone https://github.com/yilanwuyu/chatgpt-html.git

复制

然后我们调整一下项目地址，将其放进 nginx 的网站文件下（可能有所不同），并且进入到该地址：

# 将项目移动到 /var/www/html/ 目录下

mv chatgpt-html/* /var/www/html/

# 进入该目录

cd /var/www/html/

复制

设置 OpenAI 密钥

接下来，我们需要把项目文件中，index.html 文件第 47 行的密钥修改为自己在 OpenAI 申请的 API 密钥：OpenAI API

要想问我怎么注册？嘿嘿嘿，动动小手就能搜到啦～

vim index.html

复制
修改index.html文件第47行的密钥 

将sk-123456 改为 你在open ai申请的密钥 

https://beta.openai.com/account/api-keys
点击按钮创建一个 Key ，注意保存好这个 Key ，它将只出现一次。

设置完成后，我们按键盘的 ESC 键，并输入：
:wq

复制

尾声

此时，我们就已经能通过轻量应用服务器的公网 IP 地址访问刚刚搭建的 ChatGPT 了，轻量应用服务器控制台现已支持轻量域名管理，可以快速地将域名解析到您的轻量应用服务器上，如此一来，您就可以将域名分享出去，为想要玩 ChatGPT 的大家造福了！

Tips：调用 OpenAI 的 API 是收费的哦，玩乐虽好，还得注意成本。
