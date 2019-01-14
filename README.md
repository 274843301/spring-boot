# spring-boot demo
一些spring-boot的例子备忘

linux脚本设置
启动脚本 start.sh
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
