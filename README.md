## MixFileWebDAV服务器
# 注意: 需要先安装mixfile: https://github.com/InvertGeek/MixFile
可挂载到Alist中 \
安装nodejs,输入npm i 安装依赖 \
node app.js启动服务 \
config.js中配置mixfile服务器地址和webdav端口 \
alist中创建新的webdav驱动,填写http://ip:端口即可,例如http://127.0.0.1:1900/ \
文件直链响应头x-mix-code为文件分享码 \
文件目录结构和文件分享码储存在webdav.dat文件中 \
mixfile只负责上传下载和解析分享码,即使更换mixfile服务器节点，数据也不会丢失 

相比原代码增加了简单的用户密码认证功能 \
添加认证功能的初衷是部署在服务器时防止被脚本小子扫端口
