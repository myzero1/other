
###yii2安装说明



```mk
yii2安装说明

	1、安装，国内建议用 wget -c https://getcomposer.org/download/1.3.1/composer.phar 下载，下载链接可以在 https://getcomposer.org/download/ 页面下边找到。

	2、设置composer中国镜像 php composer.phar -vvv config -g repo.packagist composer https://packagist.phpcomposer.com 详情见http://pkg.phpcomposer.com/

	3、安装必须的依赖包 php composer.phar -vvv global require "fxp/composer-asset-plugin:~1.1.2" 这里必须使用global后者后面会报错。

	4、（选）安装必须的依赖包 php composer.phar -vvv global require yidas/yii2-composer-bower-skip
	这里必须使用global后者后面会报错。

	5、安装yii2，php composer.phar -vvv create-project --prefer-dist yiisoft/yii2-app-basic basic


	问题；
		（1）、在安装过程中可能会出现有一些php函数被禁用，需要在php.ini中开启，要开启proc_open,proc_close,proc_nice,proc_terminate,leak,proc_get_status,putenv这一些函数，详情看http://www.moqifei.com/archives/1600

		（2）、在安装过程中可能需要输入git token，以方便从git上获取大量数据，git token(myzero1): bc38ee397dbefa3c5b1a3b7adf3d374d3355b4f3


```
