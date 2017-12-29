# boss app测试服 输出日志


### 测试服
* 账号 ssh -p 22 root@106.75.64.209
* 密码 Legle@#23
* 调试 tail -f  + 文件夹路径
* 测试服数据库 http://test.legle.cc:8081/
* 账号 admin
* 密码 pass


### 正式服
* 账号 ssh -p 22 root@39.108.50.172
* 密码 Legle!@#123
* 调试 tail -f  + 文件夹路径
* 测试服数据库 http://azz.leglear.com:81/
* 账号 admin
* 密码 pass

### pm2命令
* 查看 pm2 ls
* pm2 show id
* 重启：pm2 restart app
* 停用：pm2 stop app

### git命令
* GIT更新代码与提交代码
* git status -s 查看改动
* git pull origin master 下载远程改动
* git add .  提交本地改动的代码到本地库
* git commit -m “改动日志” 确实代码提交到本地库
* git push origin master “提交本地库代码到 github 远程库"
* git clone git@123.59.47.209:legle/LoveChat_Nodejs.git 克隆代码
* git checkout -b im origin/im 切换分支
* git status -s  查看本地是否有改动
* 如果没有改动 git pull 下载远程库代码到本地
* 如果有改动， 就需要 先把本地代码提交到本地库，或者把不要的代码用 git checkout . 清除本地改动
* 如果谈出 vim文本编辑框 就要敲 shitf键 + ：键  然后 输入： wq 后摁 回车键
* :q退出 vim

### oss 上传文件操作：
* 1 打开 桌面里面的 ossftp 里面的 star.command
*2 打开filezilla -
*3  登录类型： 正常
*4 - 用户：access_key_id/bucket_name 
*5 - 密码：access_key_secret
*6 如用户：LTAIDACFnyvEfVHn/app-apidoc
*7 密码：x9wvJjtxDTznUSvluRqKnTGX0yOTHs
*8 端口：2048

* apidoc 的oss链接是：http://app-apidoc.oss-cn-shanghai.aliyuncs.com/index.html

* 线上配置地址http://127.0.0.1:8192/


* apidoc -i /Users/wonderchief/Desktop/app-lover/LoveChat_Nodejs/app/controllers/ -o /Users/wonderchief/Desktop/app-lover/LoveChat_Nodejs/apidoc/ -f ".*\.js$"


* apidoc -i /Users/wonderchief/Desktop/app-lover/app/controllers/ -o /Users/wonderchief/Desktop/app-lover/apidoc/ -f ".*\.js$"
在本地打开 ossftp-1.0.2-linux-mac
在终端输入命令source start.sh



* boss直约 apidoc -i /Users/wonderchief/Desktop/app-lover/app/bosscontrollers/ -o /Users/wonderchief/Desktop/app-lover/apidoc/ -f ".*\.js$"



### 数据库命令
* faces = yield Face.find({clientId: id, mobile: {$exists: true},'meta.updatedAt':{$gte: toDay, $lt: a}}).exec()

### 更新文件到测试服
* 一般文件传输工具 FileZilla, 对应的测试服主机的文件路径为 /opt/arpt-dev，把你的更新的文件覆盖掉旧文件然后重启服务就可以完成更新了.
