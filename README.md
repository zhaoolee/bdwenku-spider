# bdwenku-spider
## 一只百度文库的爬虫 A spider of baiduwenku
#### 支持txt, word, pdf, ppt类型资源的下载

#### 分析资源所在页面的源码,获取请求资源的接口,用requests库请求资源,然后手动实现文本的拼接规则,最后把文本内容输出到脚本同级目录下的文件夹中
#### 简书详细使用说明:http://www.jianshu.com/p/8c103a566bd9

- 百度文库有一些需要下载券,才能下载的资料
- 但其实文库是允许我们预览的,可是不允许我们复制内容
- 我们只是需要里面的文字内容,对内容的样式没有什么要求

# windows平台运行

![doc.gif](http://upload-images.jianshu.io/upload_images/3203841-37359c6d87d30fa6.gif?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


# 下载器实现的功能: 
> 1.按照输入的网址,自动判断文档类型,并将下载好的资源放在相应的文件夹中
![自动分类.png](http://upload-images.jianshu.io/upload_images/3203841-89aa1c7b0b6432cb.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
> 2. 将ppt类型的文档自动转换为图片,并按原本的顺序命名保存
![image.png](http://upload-images.jianshu.io/upload_images/3203841-888adf617f164a37.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
> 3.pdf,word.txt类型的数据全部消除格式,以txt格式保存文本
![image.png](http://upload-images.jianshu.io/upload_images/3203841-aee7c55d69ac0ae9.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

# 实现效果

![下载word与pdf.png](http://upload-images.jianshu.io/upload_images/3203841-7b13b5e8dee87183.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![下载ppt.png](http://upload-images.jianshu.io/upload_images/3203841-cd7fe23191b78b07.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![下载txt.png](http://upload-images.jianshu.io/upload_images/3203841-dfb7ef2dcb788b48.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 下载器的数据来源
>分析资源所在页面的源码,获取请求资源的接口,用requests库请求资源,然后手动实现文本的拼接规则,最后把文本内容输出到脚本同级目录下的文件夹中

# word类型文档
![word.png](http://upload-images.jianshu.io/upload_images/3203841-6b75f1a25c0636eb.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

# ppt类型文档
![ppt.png](http://upload-images.jianshu.io/upload_images/3203841-437f5845d6fa2445.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

# txt文档
![image.png](http://upload-images.jianshu.io/upload_images/3203841-765f678787cad9e1.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


>我把这个脚本编译成了exe文件,windows用户从下面的资源帖子里按文章名自取:
http://www.jianshu.com/p/4f28e1ae08b1

