### Linux安装MySQL

1. 更换软件源为国内镜像

2. 安装 - 执行命令: apt-get install mysql-server

3. 删除 - 执行命令: apt-get autoremove mysql-server

4. 开启远程访问

   1. 在MySQL中执行: GRANT ALL PRIVILEGES ON *.* TO 'root'@''%'' IDENTIFIED BY '你的密码';

   2.  注释掉/etc/mysql/my.cnf 中的 bind=127.0.0.1

   3. 重启MySQL服务 

      1. service mysql restart 重启服务
      2. service mysql stop 停止服务
      3. service mysql start 启动服务
