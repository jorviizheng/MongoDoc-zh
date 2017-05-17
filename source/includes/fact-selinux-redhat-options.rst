.. important::

   如果您使用 SELinux, 则必须配置 SELinux 以允许 MongoDB 在 Red Hat 系
   统上启动 (Red Hat 企业版 或 CentOS).

要配置 SELinux, 管理员有三个选项:

- 如果 SELinux 处于 ``enforcing`` 模式, 则设置允许访问 MongoDB 部署将使用的相关
  端口 (例如 ``27017`` )。有关 MongoDB 默认端口的详细信息, 请
  参阅 :doc:`/reference/default-mongodb-port` 。对于默认设置, 可以通过运行

  .. code-block:: sh

     semanage port -a -t mongod_port_t -p tcp 27017

- 通过在 ``/etc/selinux/config`` 将 ``SELINUX`` 设置为 ``disabled`` 来禁用 SELinux。

  .. code-block:: sh

     SELINUX=disabled
  
  必须重新启动系统才能使更改生效.

- 通过在 ``/etc/selinux/config`` 将 ``SELINUX`` 设置为 ``permissive`` 来将 SELinux设置
  为 ``permissive`` 模式.

  .. code-block:: sh

     SELINUX=permissive

  必须重新启动系统才能使更改生效.

  您可以用 ``setenforce`` 替换 ``permissive`` 模式。 ``setenforce`` 不需要重新
  启动, 但 **不** 是永久性的

或者, 您可以选择在安装 Linux 操作系统时不安装 SELinux 软件包, 或者选择删除相关
软件包。此选项是最危险的, 不推荐使用.
