# 如何设置自己的安全电子邮件服务器

> 原文:[https://life hacker . com/how-to-set-up-your-own-secure-email-server-1848026797](https://lifehacker.com/how-to-set-up-your-own-secure-email-server-1848026797)

最近来自威瑞森的研究表明，96%的社会工程攻击都是通过电子邮件进行的，仅仅因为这个原因，你可能需要考虑增加额外的安全性。让我们讨论一下“安全邮件服务器”的定义，它的优点和缺点，以及如何设置它。

Watch

## 什么是安全的电子邮件服务器？

普通电子邮件和安全电子邮件服务器之间的主要区别是保护级别:安全电子邮件服务器具有额外的安全功能，需要花费时间和精力来设置，但比传统电子邮件服务器更有可能抵御黑客和坏人。

简单来说，*使用*安全电子邮件地址的实际行为与普通电子邮件没有太大区别——当你切换到安全电子邮件时，你不必学习任何新技能。但是，您需要确保您选择的提供商确实使用了安全的服务器。一些受欢迎的电子邮件提供商，如谷歌或微软，可能声称他们的服务是安全的，他们在某种程度上是安全的，但是这些服务不能提供与建立你自己的安全服务器相同的控制和安全水平。

一个真正安全的电子邮件服务器不能访问你的对话，不能对你进行描述，不能 向你展示有针对性的广告，也不能记录任何数据或元数据。

## 私人电子邮件服务器的利弊是什么？

与所有技术决策一样，您应该了解使用安全电子邮件服务器的好处和缺点:

**在正面:**

*   高级隐私
*   您的雇主或电子邮件提供商无法使用该服务器
*   对电子邮件管理的更多控制
*   一般电子邮件提供商缺乏的高级功能

**在反面:**

*   创建一封安全的电子邮件需要时间和精力
*   它需要更多的责任(安装软件来防止黑客攻击，学习如何保护信息)
*   它需要有足够容量的硬盘

基本上，竞争性、安全性和可靠性是创建你的私人电子邮件服务器的首要原因。

## 设置安全的电子邮件服务器

虽然建立一个安全的电子邮件服务器的想法起初看起来令人生畏，但实际上这是一个简单的过程。它确实需要一些*比特*的技术，但是 [大量的在线资源](https://www.servermania.com/kb/articles/setup-your-own-email-server/) 可以帮助你完成这个过程。

下面是一些你需要开始做的事情:

*   您将用来设置电子邮件地址的域名(yourdomain.com)
*   云服务器或专用服务器，具有1 GHz处理器、1 GB以上的RAM空间和5 GB的磁盘空间
*   [免费、开源的Mailcow软件](https://mailcow.github.io/mailcow-dockerized-docs/)

当创建个人安全电子邮件服务器时，最好使用云服务器，而企业将从拥有专用电子邮件服务器中受益。

第一个步骤是配置DNS记录。您可以使用域名注册商的DNS，按照以下步骤操作:

*   **登录**到域名注册机构
*   **将【yourdomain.com】的域名服务器**设置为您的域名注册商的域名服务器
*   设置**mail.example.com A记录**到服务器的主IP
*   将example.com的 **MX记录设置为:**mail.example.com****

如果您使用外部DNS记录，您将遵循上面列出的相同步骤，但是设置名称服务器以匹配您的外部DNS。Juts注意到，在你可以接收和发送电子邮件之前，我需要24-48小时来传播DNS记录。

以下步骤将帮助您安装邮件服务器。首先，您需要**登录您的SSH** 。然后，你需要**更新系统包**，**安装curl和git** ，下载 **docker** 和 **docket组件**并将docker设置更新为**可执行文件**。

执行这些步骤后的下一步是确保您的umask等于0022，并切换到/opt目录。您将下载 **Mailcow文件**，将它们更改到Mailcow目录中，然后**生成配置文件**。您将提取图像，运行composer文件，安装就完成了。你现在可以使用用户名admin和密码登录你的服务器了。

你需要 [创建一个唯一的密码](https://lifehacker.com/how-to-create-secure-passwords-that-arent-impossible-to-1825048324) ，然后进入配置面板设置各种电子邮件域和电子邮件地址。然后**点击邮箱标签**添加电子邮件用户。

最后，要访问邮箱，在[【http://mail.yourdomain.com/SOGo/.】](http://mail.yourdomain.com/SOGo/.)从t 这里使用webmail界面，可以收发邮件，查看日历，查看和修改通讯录。

如果你在这个过程中遇到任何问题，建议你向一个有经验的网络解决方案提供商寻求帮助——这里有大量的你可以在线访问来帮助你解决你可能遇到的任何服务器问题。