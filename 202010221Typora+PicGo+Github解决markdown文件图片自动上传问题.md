# Typora+PicGo+Github解决markdown文件图片自动上传问题

## 背景

我写博文喜欢用markdown，所写即所得，不需要额外花时间调整格式，最近又发现了Typora这一利器，爱不释手。但还有一个麻烦的地方没有解决：图片上传。以前将markdown复制到博客，图片都还要自己手工再上传一次，太麻烦。现在找到了PicGo + Github可以几乎完美的解决这个问题。

说几乎完美是因为它的确有一个缺点，就是Github的图层在国内支持并不好，会出现加载不出来的问题，需要用VPN才能正常加载。但是这个问题只在github中浏览博文存在，如果已经复制到其他博客网站并且显示正常，那以后浏览也不会有问题。因此建议，博文上传到github后还要同步到其他博客网站，方便国内浏览；如果没有VPN，可以用gitee代替github。

## 工具安装

1. Typora: https://typora.io/
2. PicGo:https://picgo.github.io/PicGo-Doc/
3. Github:https://github.com/

首先要下载安装好这些工具，github只需有账户即可

## 配置步骤

### Github:

1. 创建一个repo，用于存储markdown文件的图片。

   ![image-20210221233331061](https://raw.githubusercontent.com/Hawking8su/Images/main/20210222001952.png)

2. 获取一个Token，用在PicGo中上传图片，步骤见下图

   注意：获取Token后一定要额外保存，因为Token内容只会展示一次，Github是不会保存的。

   ![image-20210221233455807](https://raw.githubusercontent.com/Hawking8su/Images/main/20210222001953.png)

   ![image-20210221233701202](https://raw.githubusercontent.com/Hawking8su/Images/main/20210222001954.png)

   

### PicGo App:

1. 配置Github图床

   ![image-20210221234015163](https://raw.githubusercontent.com/Hawking8su/Images/main/20210222001955.png)

2. 修改PicGo默认配置

   ![image-20210221234206664](https://raw.githubusercontent.com/Hawking8su/Images/main/20210222001956.png)

3. 验证图片上传到Github成功

   ![image-20210221234725497](https://raw.githubusercontent.com/Hawking8su/Images/main/20210222001957.png)

### Typora:

1. 配置图像上传服务

   ![image-20210221234407130](https://raw.githubusercontent.com/Hawking8su/Images/main/20210222001958.png)

   插入图片时：建议按照上图来配置，否则本地图片全部堆积在Typora默认路径，不利于管理。

   **上传服务设定：注意两点：**

    1. **PicGo的安装路径最好不要有Program Files,否则可能出现找不到PicGo.exe的报错**，这个很奇怪，我的确改了安装路径就好了，建议可参考我的安装路径。

    2. 验证图片上传选项时，如果**报错Failed to fetch，很可能是Typora上传端口与PicGo-Server端口不对应问题**，按下图步骤来验证。

       ![image-20210221235853482](https://raw.githubusercontent.com/Hawking8su/Images/main/20210222001959.png)

       ![image-20210222000924311](https://raw.githubusercontent.com/Hawking8su/Images/main/20210222002000.png)

2. 以上验证成功，就可以批量图片自动上传了

   ![image-20210221234458069](https://raw.githubusercontent.com/Hawking8su/Images/main/20210222002001.png)

   3. 最后将markdown文件上传到Github中，就可以看到有图的美博文了。然后直接复制到其他平台都会自动带图，非常方便，效率提升大大的。


以上步骤虽然还是有些麻烦，但是给我未来写博文带了更多的流畅体验，节省的时间必定可以抵掉这段研究的时间，希望能对各位博主有帮助。

参考链接：	

1. 官方配置文档：[Typora解决图片自动上传问题](https://support.typora.io/Upload-Image/)
2. 官方配置文档：[PicGo App配置Github图床](https://picgo.github.io/PicGo-Doc/zh/guide/config.html#github%E5%9B%BE%E5%BA%8A)
3. [手把手教你用Typora自动上传到picgo图床【教程与排坑】](https://www.jianshu.com/p/4cd14d4ceb1d)
4. [使用Typora+PicGo+gitee快速编辑](https://www.jianshu.com/p/f6ccdae3c95c)