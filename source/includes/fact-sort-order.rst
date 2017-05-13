在比较不同 :ref:`BSON 类型 <bson-types>` 的值时, MongoDB 使用以下比较顺序,
从最低到最高:

#. MinKey (内部类型)
#. Null
#. 数字 (ints, longs, doubles, decimals)
#. 符号, 字符串
#. 对象
#. 数组
#. 二进制数据
#. ObjectId
#. 布尔值
#. 日期
#. 时间戳
#. 正则表达式
#. MaxKey (内部类型)
