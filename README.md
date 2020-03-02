
## 框架说明
该框架主要优化提升性能，以便于更好的支持基础开发和扩展开发。
[详细请见](http://www.webpe.cn)


## ThinkPHP5.1说明
[原版新特性](https://www.kancloud.cn/thinkphp/thinkphp5_new_features/317739)
[升级指导](https://www.kancloud.cn/thinkphp/thinkphp5_new_features/317742)


## WebPE框架优化记录：
+ library\think\view\driver\Think.php 系统视图实现模板引擎按需加载
+ library\think\Log.php(89)写日记时才加载驱动
+ library\think\App.php 增加webpe路径,修改config|route|extend路径
+ library\think\App.php(200,992)增加webpe_path
+ library\think\App.php(295,300)目录调整common.php改到webpe目录命名为functions
+ library\think\console\command\optimize\Config.php(78,86) 与上面一样
+ library\think\App.php(359)注释了默认view初始化，只有继承Controller才初始化
+ library\think\App.php(360)开启调试才初始化Debug
+ library\think\App.php(989)增加方法getWebpePath
+ library\think\Loader.php(105)添加注册webpe命名空间
+ library\think\Console.php(148)目录调整command.php改到webpe目录
