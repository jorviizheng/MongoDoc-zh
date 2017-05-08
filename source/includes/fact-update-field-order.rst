.. order-of-document-fields

MongoDB 保留了写入操作后的文档字段的顺序,  *但以下情况除外* :

-  ``_id`` 字段始终是文档中的第一个字段。.

- 包含 :update:`重命名 <$rename>` 字段名称的更新可能会导致
  文档中的字段重新排序.

.. versionchanged:: 2.6

   从版本2.6 开始, MongoDB 主动尝试保留
   文档中的字段顺序。在版本2.6 之前, MongoDB 没有
   主动保留文档中字段的顺序。
