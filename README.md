自学Git笔记(来自尚硅谷课程)
========
本自学内容概述
-----

- Self-learning git and github related knowledge (covering GitHub\Gitee code cloud\GitLab) Based on version `2.31.1`, we will start from the most basic common commands to the integration of Git with development tools, how to collaborate with teams in `GitHub`, the use of `Gitee Code Cloud`(a domestic code hosting center) and the deployment of `GitLab server`(a self-built code hosting platform on LAN).
- 基于`2.31.1`版本讲解,从最基础的常用命令开始讲起，到开发工具集成`Git` 、`GitHub`如何进行团队协作、国内代码托管中心`Gitee`码云的使用、局域网自建代码托管平台`GitLab`服务器的部署
- [Git视频 尚硅谷Git入门到精通全套教程（涵盖GitHub\Gitee码云\GitLab）](https://www.bilibili.com/video/BV1vy4y1s7k6?p=8&spm_id_from=pageDriver)
- 课程自学资料链接：https://pan.baidu.com/s/1fkVj-MoCaZmyJT3q1vJmfQ  提取码：mb10
[![Git](https://cdn.learnku.com/uploads/images/201911/20/1/tcnsXi0G1J.png!large)](https://git-scm.com/)

### Git 概述
Git 是一个免费的、开源的分布式版本控制系统，可以快速高效地处理从小型到大型的各种项目。<br>
Git 易于学习，占地面积小，性能极快。 它具有廉价的本地库，方便的暂存区域和多个工作流分支等特性。其性能优于 Subversion、CVS、Perforce 和 ClearCase 等版本控制工具。

### 分布式版本控制工具
>Git、Mercurial、Bazaar、Darcs…… <br>
>
>>像 Git 这种`分布式版本控制工具`，客户端提取的不是最新版本的文件`快照`，而是把代码
仓库完整地`镜像`下来（本地库）。这样任何一处协同工作用的文件发生故障，事后都可以用
其他客户端的本地仓库进行恢复。因为每个客户端的每一次文件提取操作，实际上都是一次
对整个文件仓库的完整备份。<br>

>>`分布式`的版本控制系统出现之后,解决了`集中式`版本控制系统的缺陷:
>>>1. 服务器断网的情况下也可以进行开发（因为版本控制是在本地进行的）
>>>2. 每个客户端保存的也都是整个完整的项目（包含历史记录，更加安全）

### 常用命令
|命令名称 |作用|
|----|----|
|git config --global user.name 用户名 |设置用户签名|
|git config --global user.email 邮箱 |设置用户签名
|git init |初始化本地库
|git status |查看本地库状态
|git add 文件名 |添加到暂存区
|git commit -m "日志信息" 文件名 |提交到本地库
|git reflog |查看历史记录
|git reset --hard 版本号 |版本穿梭
