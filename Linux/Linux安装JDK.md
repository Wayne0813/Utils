### Linux安装JDK

1. 本地下载jdk-8u131-linux-x64.tar.gz安装包

2. 将下载的安装包放到服务器: /use/local/ 路径下

3. 在: /use/local/ 路径下执行: tar zvxf jdk-8u131-linux-x64.tar.gz 解压安装包

4. 执行: mv jdk... jdk8 为解压后目录重命名

5. 执行命令: vim /etc/profile 打开配置文件

6. 在打开后的文件上方添加如下内容: 

   ~~~ java
   export JAVA_HOME=/usr/local/jdk8
   export PATH=.:$JAVA_HOME/bin:$PATH
   ~~~

7. 执行命令: source /etc/profile 是配置生效

8. 执行java javac java -version 等命令校验是否成功

