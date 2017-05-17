.. admonition:: IBM POWER 系统 Ubuntu 16.04 所需的软件包更新
   :class: warning

   由于在 Ubuntu 16.04 的旧版本的 ``glibc`` 软件包中存在锁定 elision bug, 因此
   您必须在运行 MongoDB 之前将 glibc 软件包升级到至少 ``glibc 2.23-0ubuntu5`` 。具
   有较早版本的 ``glibc`` 软件包的系统将会遇到数据库服务器崩溃和错误的错误, 因为
   随机内存损坏, 不适合于部署 MongoDB 的生产环境。
