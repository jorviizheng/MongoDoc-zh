在 MongoDB 中, 存储在集合中的每个文档都需要一个充当 :term:`primary key`的
唯一字段 :term:`_id` 。如果插入的文档省略了  ``_id``  字段, 则 MongoDB 驱
动程序会自动为 ``_id`` 字段生成 :ref:`objectid` 。

这也适用于通过 update 操作的 :ref:`upsert: true <upsert-parameter>` 插入
的文档。