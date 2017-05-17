默认情况下, MongoDB 实例将其数据文件存储在 |mongod-datadir| 中,日志
文件存储在 ``/var/log/mongodb`` 中, 并使用 |mongod-user| 用户帐户
运行。您可以指定备用的日志和数据文件目录在 ``/etc/mongod.conf`` 。请
参见 :setting:`systemLog.path` 和 :setting:`storage.dbPath` 获取更多信息.

如果您更改了运行 MongoDB 进程的用户, 则 **必须** 将 |mongod-datadir| 和
``/var/log/mongodb`` 目录的访问权限设置正常, 以使该用户能够访问这些目录。
