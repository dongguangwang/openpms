# PMS统一权限管理系统
permission management system 支持多应用的统一权限管理系统，flask+vue实现

# 克隆
```
git clone https://github.com/fish2018/pms.git
# 后端
cd backend
# 前端
cd frontend
```

# 后端

## 使用方法

### 修改配置
修改app/config/settings.py使用开发环境配置
```
APP_ENV = DevelopmentConfig
```
修改app/config/dev.py根据自己情况设置数据库等信息，数据库提前创建好
```
SQLALCHEMY_DATABASE_URI = 'mysql+pymysql://root:123456@127.0.0.1:3306/PMS?charset=utf8mb4'
```

### 运行程序，默认监听host='0.0.0.0', port='5000'
python3 run.py

### 创建第一个用户，PMS默认第一个用户为管理员
http://127.0.0.1:5000打开swagger，在页面创建用户 username: admin password: admin
![](https://raw.githubusercontent.com/fish2018/pms-template/master/img/backend.jpg)

### 一些细节实现相关文章

标题：利用二进制位运算实现权限控制

地址：http://www.devopser.org/articles/2019/04/24/1556061973923.html

标题：Tree组件数据结构相互转换 flat <=> nested

地址：http://www.devopser.org/articles/2019/04/29/1556524023536.html

标题：根据用户权限动态生成菜单路由

地址：http://www.devopser.org/articles/2019/04/29/1556524856420.html