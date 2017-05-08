BSON文档最大尺寸为16M.

最大文档大小有助于确保单个文档不能使用过多的 RAM, 或者在传输过
程中占用过多的带宽. 为了存储大于最大大小的文档, MongoDB 提供
了 GridFS API. 有关 GridFS 的详细信息, 请参
阅 :program:`mongofiles` 和 :doc:`driver </applications/drivers>` 程序的文档。
