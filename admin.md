# 管理后台交接文档


### 后台代码部署路径 /opt/www/azzAdmin
* 测试服地址 http://test.legle.cc/azzAdmin/index.html#/
* 账号 jige/chengge
* 密码 123

### 后台代码放在Admin文件夹 在电脑桌面
* 测试服地址 http://test.legle.cc/azzAdmin/index.html#/
* 账号 jige/chengge
* 密码 123

* 正式服地址 http://azz.leglear.com/azzAdmin/index.html#/
* 账号 jige/chengge
* 密码 123

### 文件目录
#### 整个文件
![](http://azz-test.oss-cn-shenzhen.aliyuncs.com/admin/cCCwzaXREdSSMyQBw6wn2axH3hKhx5kC%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7+2017-12-29+%E4%B8%8B%E5%8D%886.06.09.png)  

#### src目录结构
![](http://azz-test.oss-cn-shenzhen.aliyuncs.com/admin/cCCwzaXREdSSMyQBw6wn2axH3hKhx5kC%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7+2017-12-29+%E4%B8%8B%E5%8D%886.06.23.png)  
* api存放接口
* assets存放image或者字体图标
* components存放公共组件
* main入口函数
* page主要页面（主要修改这个地方）
* router是路由
* store是vuex
* style是样式

#### 测试或者打包
* 在aizhazheng目录下运行 npm run dev 本地测试
* 在aizhazheng目录下运行 npm run build 打包压缩 会生成manage文件夹 可以发布到 /opt/www/azzAdmin

### 测试服fileZilla
* 账号 ssh -p 22 root@106.75.64.209
* 密码 Legle@#23
* 调试 tail -f  + 文件夹路径
* 测试服数据库 http://test.legle.cc:8081/
* 账号 admin
* 密码 pass


### 正式服fileZilla
* 账号 ssh -p 22 root@39.108.50.172
* 密码 Legle!@#123
* 调试 tail -f  + 文件夹路径
* 测试服数据库 http://azz.leglear.com:81/
* 账号 admin
* 密码 pass


