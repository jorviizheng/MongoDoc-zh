MongoDB 在自己的存储库中提供了正式支持的企业包。此存储库包含以下包:

.. list-table::
   :widths: 25 75

   * - ``mongodb-enterprise``
     - 将自动安装下面列出的四组件包的 ``metapackage`` .

   * - ``mongodb-enterprise-server``
     - 包含 :program:`mongod` 守护进程以及关联的配置和初始化脚本.

   * - ``mongodb-enterprise-mongos``
     - 包含 :program:`mongos` 守护进程.

   * - ``mongodb-enterprise-shell``
     - 包含 :program:`mongo` shell.

   * - ``mongodb-enterprise-tools``
     - 包含以下 MongoDB 工具: :program:`mongoimport`
       :program:`bsondump`, :program:`mongodump`, :program:`mongoexport`,
       :program:`mongofiles`, :program:`mongooplog`,
       :program:`mongoperf`, :program:`mongorestore`, :program:`mongostat`,
       and :program:`mongotop`.
