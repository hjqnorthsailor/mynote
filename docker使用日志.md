## docker使用日志
***
* nginx安装命令：docker pull nginx
* nginx启动命令：docker run --name my-nginx -d -p 80:80 -v E:/docker/webroot:/usr/share/nginx/html:ro -v E:/docker/logs:/var/log/nginx -d nginx
  绑定到80端口，挂在到E:/docker/webroot下，日志文件挂载到E:/docker/logs