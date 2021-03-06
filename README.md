<div align=center><h1>加速Github访问</h1></div>
<div align=center><p style='font-size:15px'>走出心理阴影(皮)</p></div>


## 原理

通过向提供Web请求的DNS服务器请求针对本地最优的DNS解析数据,把输出数据存入hosts文件，提高本地访问速度

## 使用

请使用Python3执行

```
git clone https://github.com/zzh-blog/GithubSpeedUp.git
cd GithubSpeedUp
python GSU.py [command]
```
查看帮助
```
python GSU.py help
```

Help文档
```
[command]:
     help         (帮助你查找帮助文档)
     add [domain] (添加待检测域名)
      └┈┈ add -y  (跳过确认部分)
     ls           (输出域名列表)
     rm [id]      (删除域名)
      └┈┈ rm -y   (跳过确认部分)
     do [id]      (输出hosts,默认是选择全部id)
     save [file]  (保存hosts)
     IPs [id]     (输出所有域名的ip,默认是选择全部id)
```

地址列表[可能存在多组地址]
```
github.global.ssl.fastly.net |67.228.235.91|
github.com |52.74.223.119|
assets-cdn.github.com |185.199.109.153|185.199.110.153|185.199.108.153|185.199.111.153|
documentcloud.github.com |185.199.109.153|185.199.111.153|185.199.110.153|185.199.108.153|
gist.github.com |203.98.7.65|
help.github.com |185.199.110.154|185.199.109.154|185.199.108.154|185.199.111.154|
nodeload.github.com |13.229.189.0|
raw.github.com |151.101.196.133|
status.github.com |54.85.97.34|52.205.36.92|52.87.114.63|
training.github.com |140.82.114.18|
www.github.com |52.74.223.119|
avatars0.githubusercontent.com |151.101.40.133|
avatars1.githubusercontent.com |151.101.40.133|
github.githubassets.com |185.199.111.154|185.199.109.154|185.199.108.154|185.199.110.154|
github-production-release-asset-2e65be.s3.amazonaws.com |52.216.88.11|
api.github.com |13.250.94.254|
user-images.githubusercontent.com |151.101.196.133|
raw.githubusercontent.com |151.101.40.133|
gist.githubusercontent.com |151.101.24.133|
cloud.githubusercontent.com |151.101.40.133|
camo.githubusercontent.com |151.101.196.133|
avatars2.githubusercontent.com |151.101.40.133|
avatars3.githubusercontent.com |151.101.24.133|
avatars4.githubusercontent.com |151.101.40.133|
avatars5.githubusercontent.com |151.101.196.133|
avatars6.githubusercontent.com |151.101.40.133|
avatars8.githubusercontent.com |151.101.24.133|
github.io |185.199.110.153|185.199.109.153|185.199.111.153|185.199.108.153|
avatars7.githubusercontent.com |151.101.24.133|
```

南京地区获取的hosts
```
199.59.148.209 github.global.ssl.fastly.net
52.74.223.119 github.com
185.199.110.153 assets-cdn.github.com
185.199.109.153 documentcloud.github.com
243.185.187.39 gist.github.com
185.199.109.154 help.github.com
54.251.140.56 nodeload.github.com
151.101.196.133 raw.github.com
52.87.114.63 status.github.com
140.82.113.17 training.github.com
13.229.188.59 www.github.com
151.101.40.133 avatars0.githubusercontent.com
151.101.196.133 avatars1.githubusercontent.com
185.199.108.154 github.githubassets.com
52.216.207.123 github-production-release-asset-2e65be.s3.amazonaws.com
54.169.195.247 api.github.com
151.101.40.133 user-images.githubusercontent.com
151.101.40.133 raw.githubusercontent.com
151.101.196.133 gist.githubusercontent.com
151.101.40.133 camo.githubusercontent.com
151.101.40.133 avatars2.githubusercontent.com
151.101.40.133 avatars3.githubusercontent.com
151.101.196.133 avatars4.githubusercontent.com
151.101.40.133 avatars5.githubusercontent.com
151.101.196.133 avatars6.githubusercontent.com
151.101.40.133 avatars8.githubusercontent.com
185.199.108.153 github.io
151.101.40.133 avatars7.githubusercontent.com
```