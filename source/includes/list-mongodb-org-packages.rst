.. Only include this file on a page containing the section title
.. "Run MongoDB Community Edition"

MongoDB 在自己的存储库中提供了正式支持的软件包。此存储库包含以下软件包:

.. list-table::
   :widths: 25 75

   * - ``mongodb-org``
     - 将自动安装下面列出的四组件软件包的  ``metapackage`` .

   * - ``mongodb-org-server``
     - 包含 :program:`mongod` 守护程序和相关的配置和 init 脚本。

   * - ``mongodb-org-mongos``
     - 包含 :program:`mongos` 守护进程.

   * - ``mongodb-org-shell``
     - 包含 :program:`mongo` shell.

   * - ``mongodb-org-tools``
     - 包含以下 MongoDB 工具: :program:`mongoimport`
       :program:`bsondump`, :program:`mongodump`, :program:`mongoexport`,
       :program:`mongofiles`, :program:`mongooplog`,
       :program:`mongoperf`, :program:`mongorestore`, :program:`mongostat`,
       and :program:`mongotop`.

``mongodb-org-server`` 软件包提供了一个初始化脚本,
使用配置文件 ``/etc/mongod.conf`` 启动 :program:`mongod` .

.. Links to the section in the including page having this title.

有关使用此初始化脚本的详细信息, 请参见运 `运行 MongoDB 社区版`_ .
