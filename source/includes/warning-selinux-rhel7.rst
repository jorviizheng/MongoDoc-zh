.. warning::

   在 RHEL 7.0 上, 如果您更改了数据路径, 没有更改安全上下文, *默认的* SELinux 策略将
   阻止 :program:`mongod` 在新数据路径上具有写权限.
