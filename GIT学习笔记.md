# git学习笔记

## 基本的linux命令学习

1) cd  更改目录

2) cd..  回到上一个目录
3) pwd 显示当前所在目录
4) ls(ll) 列出当前目录的所以文件，ll列出的更详细
5) touch 新建一个文件例如 touch XXX.X；建立XXX.X
6) rm 删除一个文件
7) mkdir 新建一个目录，就是文件夹
8) rm -r 删除一个文件夹，例如rm -r .git  删除.git目录
9) mv 移动文件
10) reset 重新出山终端/清屏
11) clear 清屏
12) history 查看历史记录
13) help 帮助
14) exit 退出
15) #表注释

# git配置

```bash
git config -l #查看配置
git config -system -list #系统配置
git config --global --list #本地配置
git config --globa1 user.name "cZz" #名称
git config --global user.email 1976644720@qq.com #邮箱
```

## git基本理论

Git本地有三个工作区域:工作目录( Working Directory)、暂存区(Stage/Index)、 资源库(Repository或Git Directory)。如果在加上远程的git仓库(Remote Directory)就可以分为四个工作区域。文件在这四个区域之间的转换关系如下:

![image-20220419002320924](C:\Users\19766\AppData\Roaming\Typora\typora-user-images\image-20220419002320924.png)

## git项目搭建

### 创建工作目录与常用指令

工作目录( WorkSpace)-般就是你希望Git帮助你管理的文件夹,可以是你项目的目录,也可以是一一个空目录 ,建议不要有中文。

日常使用只要记住下图6个命令:

![image-20220419002501177](C:\Users\19766\AppData\Roaming\Typora\typora-user-images\image-20220419002501177.png)

### 创建本地仓库

1、创建全新的仓库,需要用GIT管理的项目的根目录执行:

```bash
#在当前目录新建一个Git代码库
$ git init
```

2、执行后可以看到,仅仅在项目目录多出了- -个.git目录,关于版本等的所有信息都在这个目录里面。

### 克隆远程仓库

1、另一种方式是克隆远程目录,由于是将远程服务器上的仓库完全镜像一 份至本地! 

```bash
#克隆一个项目和它的整个代码历史(版本信息)
$ git clone [ur1] https ://gitee. com/kuangstudy/openclass. git
```

2、去gitee或者github.上克隆-一个测试 !
