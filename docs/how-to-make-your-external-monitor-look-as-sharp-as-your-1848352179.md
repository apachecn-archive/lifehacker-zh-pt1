# 如何让您的外部显示器看起来像您的高分辨率Mac显示器一样清晰

> 原文:[https://life hacker . com/how-to-make-your-external-monitor-look-as-sharp as-your-1848352179](https://lifehacker.com/how-to-make-your-external-monitor-look-as-sharp-as-your-1848352179)

自从苹果在2012年将Retina显示屏引入Mac以来，他们的大多数产品都配备了激光锐利、令人愉悦的清晰屏幕。无论你有一个小的12英寸的笔记本电脑显示器还是一个大的27英寸的台式机，你的Mac看起来可能*很棒*。因此，当你将它插入外部显示器时，看到的是模糊的文本，这可能会令人沮丧。这是怎么回事？

Watch

## 分辨率和像素使文本在Mac上更清晰

文本和图形在Mac显示器上看起来如此清晰的主要原因是分辨率和像素。苹果生产非常高分辨率的显示器；例如，M1 iMac的尺寸为4480 x 2520，分辨率大约为4K，每英寸像素为218。M1 MacBook Air采用了2560 x 1600分辨率的显示器，ppi为227，这使它处于2.5K的范围内。

你的Mac发送到显示器上的图像被放大(稍后会有更多介绍)以匹配所有这些额外的像素；结果是更清晰的文本和图像，你几乎不可能看到那些单个的T2像素。

这一切看起来都很棒...在你的Mac上，但是当你连接到一个外部显示器时，一切都可能变成垃圾。这可能是因为你连接的显示器没有清晰再现文本所需的像素数量(例如标准的1080p显示器)，或者它不是苹果标准分辨率或显示器尺寸，例如1440p或超宽显示器。

## 1080p显示器不显示清晰文本

如果你连接的是1080p的显示器，我很抱歉地告诉你，没什么可做的。虽然这些显示器工作得很好，在某些用途上看起来很棒，但它们无法像像素密度更高的显示器那样清晰地显示文本。如果清晰的文字对你真的很重要，你最好升级到更清晰的显示器。正如你将看到的，一个标准的4K显示器将是macOS最简单的解决方案，当你连接时会给你清晰的文本。

但是，升级后的外接显示器可能无法解决您的所有问题。传统的4K显示器应该没有任何问题，但是1440p显示器和超宽显示器仍然会有问题。也许你有这样的一个，你想知道为什么你的文本看起来还是模糊的。一台Windows笔记本电脑连接到这些显示器上看起来很好；为什么你的MacBook没有？

## 缩放问题会使外部显示器上的文本模糊不清

这里的一个大问题是伸缩性。当您向显示器(包括电脑的内建显示器)发送视频信号时，您可以更改信号的大小，以更好地匹配显示器。假设你有一台M1 iMac。C 选择原生4480 x 2520缩放分辨率(完全匹配显示器的分辨率)将使其基本上无法使用。一切都是*的方式*太小。将分辨率缩放到2240 x 1260左右，会使屏幕上的尺寸翻倍，但像素仍然匹配。

在1440p显示器上，您通常可以选择1080p缩放选项来保持清晰的像素外观。Mac的情况并非如此。出于某种原因，苹果公司使得1440p和超宽显示器输出视网膜信号似乎是不可能的。与Windows不同，macOS没有完成工作所需的扩展选项。

## 如何在1440p或超宽显示器上锐化Mac文本

如果这听起来像是你的问题，有几个修复方法可以尝试。首先，看看禁用字体平滑是否有帮助。虽然你以前可以从系统偏好设置中禁用这个选项，但苹果用Big Sur移除了它。不过，您仍然可以从终端禁用它。

首先，打开终端，然后复制并粘贴**defaults-current host write-g AppleFontSmoothing-int 0**，然后点击“Enter”此命令会停用字体平滑，这有助于使文本在1440p或超宽显示器上看起来更清晰。这里的控制器是命令末尾的数字；“0”表示禁用该功能，而使用1、2或3则稳定增加该功能的强度。您可以使用命令**默认值-当前删除-g AppleFontSmoothing** 将该特征重置为默认值。

如果那不起作用，一些人已经发现使用 [更好的虚拟](https://www.macupdate.com/app/mac/63642/betterdummy) 是成功的。此工具允许您创建一个“假”macOS窗口，然后成为外部显示器上的主窗口。使用这个工具，你可以获得比macOS默认提供的更多的缩放选项，这有助于匹配你的特定显示器。