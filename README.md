# CI_frame_php
CI框架学习


一、CI框架熟悉
——加载静态页面
1、下载框架，安装到开发环境
2、新建一个控制器来处理静态页面（新建一个文件 application/controllers/Pages.php）
   文件开头要大写，类名必须以大写字母开头。
3、新建两个视图（页面模板）分别作为我们的页脚和页头
新建页头文件 application/views/templates/header.php
新建个页脚文件 application/views/templates/footer.php 
4、 视图下新建pages文件下的home.php 和 about.php
——读取新闻条目
1、创建数据模板
2、application/models/ 目录，新建一个文件 News_model.php
3、数据库配置(application/config/database.php)更改多维数组default
         dsn	DSN 连接字符串（该字符串包含了所有的数据库配置信息）
         hostname	数据库的主机名，通常位于本机，可以表示为 "localhost"
         username	需要连接到数据库的用户名
         password	登录数据库的密码
         database	你需要连接的数据库名
         dbdriver	数据库类型。如：mysql、postgres、odbc 等。必须为小写字母。
         dbprefix	当使用 查询构造器 查询时，可以选择性的为表加个前缀， 它允许在一个数据库上安装多个 CodeIgniter 程序。
         pconnect	TRUE/FALSE (boolean) - 是否使用持续连接
         db_debug	TRUE/FALSE (boolean) - 是否显示数据库错误信息
         cache_on	TRUE/FALSE (boolean) - 是否开启数据库查询缓存， 详情请见 数据库缓存类。
         cachedir	数据库查询缓存目录所在的服务器绝对路径
         char_set	与数据库通信时所使用的字符集
         dbcollat	与数据库通信时所使用的字符规则（注解：只使用于 'mysql' 和 'mysqli' 数据库驱动）
         swap_pre	替换默认的 dbprefix 表前缀，该项设置对于分布式应用是非常有用的， 你可以在查询中使用由最终用户定制的表前缀。
         schema	数据库模式，默认为 'public'，用于 PostgreSQL 和 ODBC 驱动
         encrypt	是否使用加密连接。
         compress	TRUE/FALSE (boolean) - 是否使用客户端压缩协议（只用于MySQL）
         stricton	TRUE/FALSE (boolean) - 是否强制使用 "Strict Mode" 连接, 在开发程序时，使用 strict SQL 是一个好习惯。
         port	数据库端口号，要使用这个值，你应该添加一行代码到数据库配置数组。$db['default']['port'] = 5432;

4、 读取新闻条目
5、 创建新闻条目


二、常规专题
1、方法命名一定不能和 主程序控制器类中的方法名相同
2、
