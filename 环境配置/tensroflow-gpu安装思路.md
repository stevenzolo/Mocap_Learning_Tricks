# tensroflow-gpu安装思路


##安装流程
安装tensorflow-gpu时需要考虑各个依赖是否兼容，此处以TensorFlow1.5.0为例。

参考链接(https://blog.csdn.net/u014797226/article/details/80229887?spm=1001.2101.3001.6650.16&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7Edefault-16.no_search_link&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7Edefault-16.no_search_link)

1.gcc版本选择7.5

2.安装显卡驱动，版本450-460，一定要安装下载的那种run，需要关闭图形界面。

3.安装cuda9.0

4.安装cudnn7.0

5.安装python 3.6

6.在anaconda中安装tensorflow-gpu==1.5.0

##注意事项 :
1.安装显卡驱动失败电脑可能会打不开，解决办法就是找到之前的显卡驱动安装包在命令行下安装，如果没有安装包可以用在其他电脑里下一个用u盘装上。

2.其他版本tensorflow安装均需要考虑相应的这些依赖版本。
