# 全民K歌下载器
## 介绍
爬取指定用户的全部歌曲并下载。
## 使用方法
1. 配置好python环境以及相关库：
   ```
   import requests
   import re
   from bs4 import BeautifulSoup
   ```
2. 电脑访问指定用户的个人主页：
3. 填入相关参数：
   ```
   param = {
    'outCharset': 'utf-8',
    'from': '1',
    'nocache': '', # 换成你自己的
    'format': 'json',
    'type': 'get_uinfo',
    'start': str(num),
    'num': '15',
    'share_uid': '', # 换成你要找的那个歌手的
    'g_tk': '5381',
    'g_tk_openkey': '5381'
   }
   head = {
    'Host': 'node.kg.qq.com',
    'Cookie': '', # 换成你自己的
    'Sec-Ch-Ua': '"Chromium";v="111", "Not(A:Brand";v="8"',
    'Accept': 'application/json, text/plain, */*',
    'Sec-Ch-Ua-Mobile': '?1',
    'User-Agent': 'Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.5563.65 Mobile Safari/537.36',
    'Sec-Ch-Ua-Platform': '"Android"',
    'Origin': 'https://static-play.kg.qq.com',
    'Sec-Fetch-Site': 'same-site',
    'Sec-Fetch-Mode': 'cors',
    'Sec-Fetch-Dest': 'empty',
    'Referer': '', # 换成你自己的
    'Accept-Encoding': 'gzip, deflate',
    'Accept-Language': 'zh-CN,zh;q=0.9'
   }
   ```
5. 运行python脚本：
   ```
   python download.py
   ```
