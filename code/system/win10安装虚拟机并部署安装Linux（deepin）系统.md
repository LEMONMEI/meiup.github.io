# win10安装虚拟机并部署安装Linux（deepin）系统

-------
**本文首发于[https://www.cnblogs.com/auto-ajax/p/15478373.html](https://www.cnblogs.com/auto-ajax/p/15478373.html)**

##### 前言
1. 这是基于Hexo的博客搭建的系列内容，完全自定义开发周期太长了，先曲线救国，借个框框用用。整个系利都有参考[@卢well](https://blog.csdn.net/qq_36949103)和[hexo史上最全搭建教程](https://blog.csdn.net/sinat_37781304/article/details/82729029/)的相关内容，点击博客名可直接跳转
2. 安装虚拟机主要是用于学习在linux环境下进行应用开发，虽然我已经单独安装了linux系统在移动硬盘里，但是每次使用都需要重新启动切换，总觉得不是很方便，所以想想还是直接安装一个虚拟机吧。
3. 虚拟机软件一般使用的比较多的是VMware workstation和VirtualBox，我这次使用的是VMware workstation，之前使用过VB，可能是我电脑配置不咋跟得上，或者自己技术实在是太菜了，使用体验不是很好，这次就想着换一个平台试试。
---
**[@参考原文https://blog.csdn.net/daerzei/article/details/82919344](https://blog.csdn.net/daerzei/article/details/82919344)**
### 一、VMware workstation软件安装
&emsp;&emsp;VMware workstation因为是一款商业软件，所以一般都是需要付费的，但是为了学习，大多数人在大多数时间里都是使用的和谐版，我使用的版本是[VMware Workstation v16.1.1 中文破解版](https://www.xitmi.com/2417.html)，点击可跳转至资源界面，如果资源过期了也可联系我获取。
<br>
VM的安装很简单，按照常规的软件安装程序来就好了，建议修改一下安装路径。如果你使用的是和我一样的资源，那么破解用的注册序列号都准备好了，按照你安装的版本选择序列号就行了，正常情况安装结束就会有一个添加序列号的选项，按需复制粘贴进去就好了（我个人认为这里不需要附图，实在需要的话，留言即可，我会来补一个）。

### 二、linux系统在虚拟机VM上部署
#### 1. 先配置一下要安装系统的参数
1. 新建一个虚拟机
![](https://img2020.cnblogs.com/blog/2003558/202110/2003558-20211029203542589-261162668.png)

2. 选择典型安装
![](https://img2020.cnblogs.com/blog/2003558/202110/2003558-20211029203634525-1393278309.png)

3. 配置镜像，选择稍后安装操作系统
![](https://img2020.cnblogs.com/blog/2003558/202110/2003558-20211029204114293-1672794986.png)

4. 选择Linux系统类型，由于Deepin是在Ubuntu的基础上面向国内进行定制化开发的，所以这里Linux的版本选择了Ubuntu64位
![](https://img2020.cnblogs.com/blog/2003558/202110/2003558-20211029204243893-610654764.png)

5. 给系统起个名字，改下路径（路径看自己习惯）
![](https://img2020.cnblogs.com/blog/2003558/202110/2003558-20211029204551341-1667174423.png)

6. 设置磁盘容量
![](https://img2020.cnblogs.com/blog/2003558/202110/2003558-20211029204710750-871568477.png)

7. 自定义硬件，这个根据自己的电脑情况来配置就好了
![](https://img2020.cnblogs.com/blog/2003558/202110/2003558-20211029204803038-1950813944.png)

主要配置4项：
内存：给你要创建的虚拟机分配合适的内存
处理器：CPU数量及核数与你电脑实际的情况一致
新CD/DVD(SATA)：指定要使用的深度（Deepin）ISO镜像
网络适配器：桥接模式
我的配置如下：
![](https://img2020.cnblogs.com/blog/2003558/202110/2003558-20211029205810232-1024747759.png)

最后点击关闭完成配置，点击完成准备进入下一步安装。
#### 2. 开始安装deepin
1. 启动虚拟机，并启动安装，一般启动安装会自动跳转的
![](https://img2020.cnblogs.com/blog/2003558/202110/2003558-20211029210257864-93170923.png)
![](https://img2020.cnblogs.com/blog/2003558/202110/2003558-20211029210417700-1397457499.png)
安装步骤就和正常的Deepin安装是一样的了，只是会多一个确认，下一步即可
![](https://img2020.cnblogs.com/blog/2003558/202110/2003558-20211029210647365-539167293.png)
安装完大概就是这个样子，由于deepin版本不同，界面可能有所不同，但是流程基本就是这个流程。
![](https://img2020.cnblogs.com/blog/2003558/202110/2003558-20211029222540371-352974335.png)

<br>
关于deepin的安装步骤和过程，难度不是很大，可以试着百度直接来就好了，毕竟在虚拟机上弄错了直接删掉重新再来一下就好了，实在需要的话可以留言，我在后面补一篇deepin的安装步骤。
<br>
