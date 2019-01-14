# spring-boot demo
一些spring-boot的例子备忘

linux脚本设置
启动脚本 start.sh,nohup 为日志文件
nohup java -jar app-v1.0.jar --spring.config.location=application.yml &
<br /><br />
停止脚本 stop.sh
PID=$(ps -ef | grep app-v1.0.jar | grep -v grep | awk '{ print $2 }')
if [ -z "$PID" ]
then
echo Application is already stopped
else
echo kill $PID
kill $PID
fi
<br /><br />
新建空白Log文件，保存日志 nohup.out
<br /><br />
touch nohup.out
查看日志 log.sh

tail -f nohup.out
