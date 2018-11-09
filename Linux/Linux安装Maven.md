### Linux安装Maven

1. 更换软件源为国内镜像

2. 执行命令下载安装包: wget http://mirrors.tuna.tsinghua.edu.cn/apache/maven/maven-3/3.3.9/binaries/apache-maven-3.3.9-bin.tar.gz 

3. 执行命令: mv ./fileName /use/local/ 将下载的安装包移动到 /use/local/ 目录下

4. 执行命令解压: tar zvxf fileName

5. 执行命令: vim /etc/profile 打开配置文件

6. 在打开后的文件上方添加如下内容: 

   ~~~ java
   export M2_HOME=/usr/local/maven3
   export PATH=.:$PATH:$M2_HOME/bin
   ~~~

7. 执行命令: source /etc/profile 是配置生效

8. 执行mvn -v 检查是否安装成功