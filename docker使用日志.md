## docker使用日志
***
#### nginx
* nginx安装命令：docker pull nginx
* nginx启动命令：docker run --name my-nginx -d -p 80:80 -v E:/docker/webroot:/usr/share/nginx/html:ro -v E:/docker/logs:/var/log/nginx -d nginx
  绑定到80端口，挂在到E:/docker/webroot下，日志文件挂载到E:/docker/logs
### mysql
* 安装命令：docker pull mysql
* 启动命令： docker run -p 3307:3306 --name mymysql -v E:/docker/mysql/conf/my.cnf:/etc/mysql/my.cnf -v E:/docker/mysql/logs:/logs -v E:/docker/mysql/data:/mysql_data -e MYSQL_ROOT_PASSWORD=123456 -d mysql