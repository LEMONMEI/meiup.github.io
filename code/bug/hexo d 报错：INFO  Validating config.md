# hexo d 报错：INFO  Validating config

今天在使用hexo搭建个人博客的时候，出现一个及其令人喷血的报错：
![](https://img2020.cnblogs.com/blog/2003558/202111/2003558-20211114212341173-969775542.png)
我几乎查遍了所有有关hexo提交报错的解决办法，都！没！用！
<br>
就在我准备重装虚拟机系统的时候，扫了一眼创建文件下的配置文件推送路径：
```javascript
deploy:
  type: ''
  repo: 
    github: git@github.com:LemonMei/LemonMei.github.io.git
    # github: https://github.com/LemonMei/LemonMei.github.io.git
  branch: master

# backup
backup:
  type: git
  message: backup my blog of https://yourname.github.io/
  repository:
    github: https://github.com/LemonMei/LemonMei.github.io.git,backup
```
**TMD!!!**
我的`type`后面没有跟`git`！！！
<br>
真的绝了...
<br>
附上他正确的写法：
```javascript
deploy:
  type: git
  repo: 
    github: git@github.com:LemonMei/LemonMei.github.io.git
    # github: https://github.com/LemonMei/LemonMei.github.io.git
  branch: master

# backup
backup:
  type: git
  message: backup my blog of https://yourname.github.io/
  repository:
    github: https://github.com/LemonMei/LemonMei.github.io.git,backup
```
