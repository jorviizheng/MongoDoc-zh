.. note::

   大多数 MongoDB 驱动程序客户端将包含 ``_id`` 字段, 并在插入操作发
   送到 MongoDB 之前生成一个 ``ObjectId`` ;但是, 如果客户端发送没
   有 ``_id`` 字段的文档, 则 :program:`mongod` 将添加 ``_id`` 字段
   并生成 ``ObjectId`` 。
