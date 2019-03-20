# [Composer](http://www.phpcomposer.com/)
	Thinkphp5自带了composer.phar组件， 如果没有安装，则需要进行安装

## 安装
	> 一下命令全部在项目目录下运行
	> windows先要添加php路径到系统的环境变量中
	* php composer.phar install
	* php composer.phar selfupdate
	* php composer.phar config repo.packagist composer http://packagist.phpcomposer.com  修改源地址，使用国内源地址，提升组件安装速度

## 添加组件
	* php composer.phar require aliyuncs/oss-sdk-php 其中aliyuncs/oss-sdk-php为组件名称，组件名称可以从https://packagist.org/ 搜到

## 更新组件
	* php composer.phar update --dry-run  查看可升级的组件
	* php composer.phar update

## 卸载组件
	* php composer.phar remove aliyuncs/oss-sdk-php  卸载组件的时候会把引入的其它组件一并卸载

! (https://github.com/locoiy/doc/blob/master/imges/25f0a2bedb70de7f29f8dafe18955c33.png?raw=true)
