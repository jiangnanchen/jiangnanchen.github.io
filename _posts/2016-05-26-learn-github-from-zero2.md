---
layout: post
keywords: blog
description: blog
title: "从0开始学习 GitHub 系列之「加入 GitHub」"
categories: [GitHub]
tags: [GitHub]
---
{% include codepiano/setup %}

![](/image/github2.jpg)

看完昨天的文章「[从0开始学习 GitHub 系列之「初识 GitHub」](http://stormzhang.com/github/2016/05/25/learn-github-from-zero1/)」估计不少人已经开始期待我继续更新了，这不赶紧马不停蹄，加班加点给你们更新了第二篇。在更新本篇文章之前先回答昨天大家留言的两个问题：

- GitHub 需要翻墙么？

印象中 GitHub 之前确实总是断断续续的访问不了，不过在13年初的时候有段时间最严重，一度被封了，当时李开复老师再也忍无可忍，公开发了一条抗议 GitHub 被封的微博，这事我印象很深，因为我是12年底加入的 GitHub ，那时候简直像遇到世外桃源一般，但是也深受老是访问不了的困扰，很多人早就对这件事怨声载道了，加上李开复老师的声讨，这一下就炸开了锅，微博上纷纷转发谴责，算的上是整个IT界的大新闻，后来因为这事影响太大了，没过几天 GitHub 就可以正常访问了，这里真的要感谢李开复老师敢于站出来的勇气，可以这么说，如果没有 GitHub ，中国的编程水平起码要倒退好多年！

因为 GitHub 的影响力太大，基本上是各种黑客攻击的对象，所以现在偶尔也会有宕机访问不了的情况，但是好在不会被封，所以大家不用担心，访问 GitHub 不用翻墙，只是可能访问速度稍慢些，另外为了维护一个和谐的环境，这里也呼吁大家不要在 GitHub 上发表任何关于政治的言论与文章，在 GitHub 上我们只是单纯的技术交流，无关政治，在复杂的大环境下，希望 GitHub 永远是我们程序员的一片净土！

- 英语差、0基础学得会么？

这个也是不少人问我的，GitHub 虽然都是英文，但是对英语水平的要求不是那么高，都是些简单的单词，遇到不会的查一下就行了，你觉得很难只是你对英文网站反射性的抵触而已，相信我，跟着我的详细教程，我的文章面向从没有接触过甚至没有听过 GitHub 的同学，一步步教你由浅入深。如果你学不会，那么来打我，不过我这么帅，你也不忍心！

好了，废话不多说，咱们进入正文！

## 1. 注册 GitHub

先去 GitHub 官网「How people build software · GitHub」注册「Sign Up」个账号，注册页面如下：

![](/image/join_github1.png)

这个应该没啥说的，需要填用户名、邮箱、密码，值得一提的用户名请不要那么随便，最好取的这个名字就是你以后常用的用户名了，也强烈建议你各大社交账号都用一样的用户名，这样识别度较高，比如我的博客域名、GitHub、知乎等其他社交账号 ID 都是 stormzhang ，微博是因为被占用了，无奈换了个id，而且这个用户名以后在 GitHub 搭建博客的时候默认给你生成的博客地址就是 http://username.github.io ，所以给自己取个好点的用户名吧。

填好用户名、邮箱、密码紧接着到这一步：

![](/image/join_github2.png)

这个是什么意思呢？GitHub 有两种，一种是公开，这种是免费的，就是你创建的项目是开放的，所有人都能看得到；另一种是私有，这种是收费的，这种一般是很多企业在使用 GitHub 的私有仓库在托管自己的项目，这也是 GitHub 的一种盈利模式对于个人你就直接默认选择公开的就行了。

## 2. 认识 GitHub

注册成功之后你会到 GitHub 的主页面来：

![](/image/github_home.png)

你如果是新注册的可能看到的跟我不一样，因为你们新用户，没有自己的项目，没有关注的人，所以只有一个导航栏。

导航栏，从左到右依次是 GitHub 主页按钮、搜索框、PR、Issues、Gist（这些概念后面会讲的）、消息提醒、创建项目按钮、我的账号相关。

我的 Timeline，这部分你可以理解成微博，就是你关注的一些人的活动会出现在这里，比如如果你们关注我了，那么以后我 star、fork 了某些项目就会出现在你的时间线里。

我的项目，这部分就不用说了，如果你创建了项目，就里就可以快捷访问。


## 3. GitHub 主页

点击下图的 Your profile 菜单进入到你的个人 GitHub 主页。

![](/image/github_home2.png)

还是以我的 GitHub 主页为例：

![](/image/github_account.png)

这么详细应该不会看不懂吧？只不过你的账号可能没有这么丰富，因为你可能啥也没做过，但是如果做全了基本上就会看到跟我一样的了。

## 4. 设置你的 GitHub

如果你是新注册的 GitHub 账号，是不是觉得很简陋？虽然你没有自己的项目，但是第一步起码要先完善自己的信息，点击如下的 Settings 菜单：

![](/image/github_setting.png)

到设置页面来设置一些基本信息：

![](/image/github_profile.png)

像头像、Name 建议要设置一个常用的，这两个很有识别性，公开的邮箱也要设置一个，这样那些企业啊、猎头啊就通过这个公开邮箱去联系你，友情提醒：别在 GitHub 把自己的 QQ 邮箱放上去，不显得太 low 了么？没有 gmail 邮箱，起码也得注册个 foxmail、163 邮箱之类的吧。


## 5. GitHub 基本概念

上面认识了 GitHub 的基本面貌之后，你需要了解一些 GitHub 的基本概念，这些概念是你经常会接触并遇到的。

- Repository

仓库的意思，即你的项目，你想在 GitHub 上开源一个项目，那就必须要新建一个 Repository ，如果你开源的项目多了，你就拥有了多个 Repositories 。

- Issue

问题的意思，举个例子，就是你开源了一个项目，别人发现你的项目中有bug，或者哪些地方做的不够好，他就可以给你提个 Issue ，即问题，提的问题多了，也就是 Issues ，然后你看到了这些问题就可以去逐个修复，修复ok了就可以一个个的 Close 掉。

- Star

这个好理解，就是给项目点赞，但是在 GitHub 上的点赞远比微博、知乎点赞难的多，如果你有一个项目获得100个star都算很不容易了！

- Fork

这个不好翻译，如果实在要翻译我把他翻译成分叉，什么意思呢？你开源了一个项目，别人想在你这个项目的基础上做些改进，然后应用到自己的项目中，这个时候他就可以 Fork 你的项目，这个时候他的 GitHub 主页上就多了一个项目，只不过这个项目是基于你的项目基础（本质上是在原有项目的基础上新建了一个分支，分支的概念后面会在讲解Git的时候说到），他就可以随心所欲的去改进，但是丝毫不会影响原有项目的代码与结构。

- Pull Request

发起请求，这个其实是基于 Fork 的，还是上面那个例子，如果别人在你基础上做了改进，后来觉得改进的很不错，应该要把这些改进让更多的人收益，于是就想把自己的改进合并到原有项目里，这个时候他就可以发起一个 Pull Request（简称PR） ，原有项目创建人就可以收到这个请求，这个时候他会仔细review你的代码，并且测试觉得OK了，就会接受你的PR，这个时候你做的改进原有项目就会拥有了。

- Watch

这个也好理解就是观察，如果你 Watch 了某个项目，那么以后只要这个项目有任何更新，你都会第一时间收到关于这个项目的通知提醒。

- Gist

有些时候你没有项目可以开源，只是单纯的想分享一些代码片段，那这个时候 Gist 就派上用场了！

## 6. 创建自己的项目

点击顶部导航栏的 + 可以快速创建一个项目，如下图：

![](/image/create_repo.png)

创建一个项目需要填写如上的几部分：项目名、项目描述与简单的介绍，你不付费没法选择私有的，所以接着只能选择 public 的，之后勾选「Initialize this repository with a README」，这样你就拥有了你的第一个 GitHub 项目：

![](/image/init_repo.png)

可以看到这个项目只包含了一个 README.md 文件，但是它已经是一个完整的 Git 仓库了，你可以通过对它进行一些操作，如watch、star、fork，还可以 clone 或者下载下来。

这里提一下 README.md ，GitHub 上所有关于项目的详细介绍以及 Wiki 都是基于 Markdown 的，甚至之后在 GitHub 上搭建博客，写博客也是如此，所以如果还不懂 Markdown 语法的，建议先去学习下。推荐一篇学习 Markdown 的文章给你们：

[献给写作者的 Markdown 新手指南](http://www.jianshu.com/p/q81RER)

## 7. 总结

相信看完以上文章你已经基本算是了解 GitHub 的基本概念并且正式加入 GitHub 这个大家庭了，之后会有更深入的文章介绍 Git、介绍对项目的常用操作、介绍如何给开源项目提交代码、介绍如何协同合作甚至怎么搭建博客等，敬请期待吧！

<br />

> 本文原创发布于微信公众号 **AndroidDeveloper「googdev」**，转载请务必注明出处！

![图片描述](/image/weixinpublic.jpg)
