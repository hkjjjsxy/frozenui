### sass

写css代码用sass，win系统下需安装ruby

### nico 

需要安装[nico](http://lab.lepture.com/nico/zh/)生成文档以及调试，`nico build `命令生成文档，`nico server `命令调试


### grunt

[参考](https://github.com/QQVIPTeam/team/issues/5)

使用`grunt docs`会编译代码以及开启nico测试，访问[127.0.0.1:8000](127.0.0.1:8000)调试页面

使用`grunt --log=logtest` 命令会打包当前版本所需的包,生成如1.0.0的文件夹, 生成_site站点以及svn提交，ftp同步，git提交

css ，css-debug和img目录是需要发布到线上，_css-debug_是未压缩的版本，为调试使用

i.gtimg.cn.zip需要发布到离线包


### git

使用nico生成好的文档会在_site目录，提交当前目录到https://github.com/frozenui/baseui.git

_site目录下的内容提交到gh-pages分支，参考https://github.com/frozenui/baseui/issues/

页面会显示在frozen的css组件菜单项中http://frozenui.github.io/baseui/


### 版本管理

分为小版本和大版本，目前grunt的功能还不完善，只支持升小版本，后续会优化

小版本控制发布频率在一月一次，不新增离线包，仅在当前的离线包中增加一个新版本的文件夹，图片未修改和新增的不用copy过来

大版本则需新增离线包，修改bid，需要打包一个全新的文件夹，并且图片也要copy进来（vip的图片不用）。

