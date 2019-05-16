# codescan-server
1. 安装
   git clone https://github.com/yanghaisheng-github/codescan-server.git
   cd codescan-server
   cnpm i

2. 修改连接mysql数据库配置：
   修改./config/db.config.js目录下host的IP

3. 安装7-zip
   本项目中使用7-zip解压缩，所以电脑上需要安装7-zip，并配置环境变量
   sca的log位置：C:\Users\Administrator\AppData\Local\Fortify\sca18.2\log

4. 运行
   npm start
   或者
   supervisor -i RTF,uploads,downloads,.git  ./bin/www

5. 引用日志
var logger = require('log4js').getLogger("文件名称");
/*   logger.info("this is info");
  logger.warn("this is warn");
  logger.debug("this is debug");
  logger.error("this is error"); */