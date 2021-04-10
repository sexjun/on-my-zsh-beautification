
## 第一步：下载iterm2
去[iterm2官网](https://iterm2.com/)下载安装就好了。

当然最推荐还是brew！！！
```
brew cask install iterm2
```

## 第二步：下载仓库

本仓库包含字体，字库，主题仓库。

```git

```


## 第三部：配置
### 3.0 安装Oh My Zsh
```
  sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```


### 3.1 配置字体
- 执行如下指令安装字体
	```
	cd fonts
	./install.sh
	# clean-up a bit
	cd ..
	```
- 更换字体
	然后打开 iTerm2，按Command + ,键，打开 Preferences 配置界面，然后Profiles -> Text -> Font -> Chanage Font，选择 Meslo LG M Regular for Powerline 字体。
	![在这里插入图片描述](https://img-blog.csdnimg.cn/20210411014240541.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NleHlsdW5h,size_16,color_FFFFFF,t_70)
### 3.2 配置主题
在下载的代码里有一个iTerm2-Color-Schemes的文件夹
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210411020108992.png)
这个文件的内部：schemes子文件里面有很多主题，可以自行选择。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210411020236863.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NleHlsdW5h,size_16,color_FFFFFF,t_70)

- setting path
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210411003505133.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NleHlsdW5h,size_16,color_FFFFFF,t_70)
- schemes path
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210411004457830.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NleHlsdW5h,size_16,color_FFFFFF,t_70)
- seeting color scheme
	after you import the scheme you like, it will shows in here![after you import the scheme you like, it will shows in here](https://img-blog.csdnimg.cn/20210411004636810.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NleHlsdW5h,size_16,color_FFFFFF,t_70)


### 3.3 配置高亮度
执行如下指令
```
echo "source ${(q-)PWD}/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc
```

### 3.4 配置提醒



@[toc]
## on-my-ssh
### 介绍

shell的类型有很多种，linux下默认的是bash，虽然bash的功能已经很强大，但对于以懒惰为美德的程序员来说，bash的提示功能不够强大，界面也不够炫，并非理想工具。

而zsh的功能极其强大，只是配置过于复杂，起初只有极客才在用。后来，有个穷极无聊的程序员可能是实在看不下去广大猿友一直只能使用单调的bash, 于是他创建了一个名为oh-my-zsh的开源项目...

![在这里插入图片描述](https://img-blog.csdnimg.cn/20210411005011118.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NleHlsdW5h,size_16,color_FFFFFF,t_70)
## 安装
查看系统当前使用的shell
```
$ echo $SHELL 
/bin/bash
```

查看shell列表

`$ cat /etc/shells `
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210411005153713.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NleHlsdW5h,size_16,color_FFFFFF,t_70)
- [on-my-zsh github 地址](https://github.com/ohmyzsh/ohmyzsh)

三种安装方式任意选一种。
- curl	`sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
- wget	`sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
- fetch	`sh -c "$(fetch -o - https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

安装成功的界面。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210411005542440.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NleHlsdW5h,size_16,color_FFFFFF,t_70)

## 主题美化
- download the color schemes
[GitHub url](https://github.com/mbadolato/iTerm2-Color-Schemes)
> - you can just donwload like by using
> - ` git clone git@github.com:mbadolato/iTerm2-Color-Schemes.git`
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210411003359911.png)
	
after you download ,you can see the color schemes in the file readme 
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210411004223425.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NleHlsdW5h,size_16,color_FFFFFF,t_70)


Use it as follows。

- setting path
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210411003505133.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NleHlsdW5h,size_16,color_FFFFFF,t_70)
- schemes path
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210411004457830.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NleHlsdW5h,size_16,color_FFFFFF,t_70)
- seeting color scheme
	after you import the scheme you like, it will shows in here![after you import the scheme you like, it will shows in here](https://img-blog.csdnimg.cn/20210411004636810.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NleHlsdW5h,size_16,color_FFFFFF,t_70)
## 字体安装

[github 链接](https://github.com/powerline/fonts)

下载后执行
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210411014007149.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NleHlsdW5h,size_16,color_FFFFFF,t_70)

更换字体：

然后打开 iTerm2，按Command + ,键，打开 Preferences 配置界面，然后Profiles -> Text -> Font -> Chanage Font，选择 Meslo LG M Regular for Powerline 字体。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210411014240541.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NleHlsdW5h,size_16,color_FFFFFF,t_70)



