## 在Windows上安装Ubuntu双系统

### 一篇博客：[windows10安装ubuntu双系统教程（绝对史上最详细）](https://www.cnblogs.com/masbay/p/10745170.html)

如果进入系统前出现花屏很可能是独立显卡的原因（未安装ubuntu下的独立显卡驱动，所以此时应该不使用独立显卡），参考[博客](https://www.jianshu.com/p/df7bb3d7be03)：

 - 进入开机boot选项界面（F12，ESC……不同电脑有差别）
 - 在ubuntu boot选项处按e，进入boot编辑界面
 - 找到linux一行，在quiet splash处后加上 nomodeset，这样就不会使用NVIDIA显卡
 - Ctrl+X保存并重新启动
 - 进入Ubuntu系统后安装NVIDIA显卡驱动
![](%E7%A9%BA%E7%99%BD_md_files%5Cimage.png?v=1&type=image)
![](%E5%9C%A8Windows%E4%B8%8A%E5%AE%89%E8%A3%85Ubuntu%E5%8F%8C%E7%B3%BB%E7%BB%9F_md_files%5Cimage%20%283%29.png?v=1&type=image)

