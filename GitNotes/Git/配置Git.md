# 配置 Git

## 安装 Git
*  在[官网](https://git-scm.com/downloads)下载适合的 Windows 版软件
* 安装 Git 并选择所有默认选项

安装完毕后，你应该能够在命令行工具中运行 git

## 配置命令提示符
[下载](http://video.udacity-data.com.s3.amazonaws.com/topher/2017/March/58d31ce3_ud123-udacity-terminal-config/ud123-udacity-terminal-config.zip)配置文件 | [本地备份](_v_attachments/20191120202230884_27657/ud123-udacity-terminal-config.zip)

[在 操作教程 Windows 上配置命令提示符.mp4](_v_attachments/20191120202230884_27657/在%20Windows%20上配置命令提示符.mp4)

## 初次配置 Git
参考：
* [初次运行 Git 前的配置](https://gitee.com/help/articles/4107)
* [First-Time Git Setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup) | [中](https://git-scm.com/book/zh/v2/起步-初次运行-Git-前的配置)

在开始使用 Git 之前，你需要配置 Git。在命令行工具中运行以下每行，确保所有选项都已被配置好。

```shell
# 设置你的 Git 用户名
git config --global user.name "<Your-Full-Name>"

# 设置你的 Git 邮箱
git config --global user.email "<your-email-address>"

# 确保 Git 输出内容带有颜色标记
git config --global color.ui auto

# 对比显示原始状态
git config --global merge.conflictstyle diff3

# 列出所有的配置
git config --list
```

## Git 与代码编辑器
配置 Git 使其能与你的代码编辑器结合使用。

```shell
# VSCode 设置
git config --global core.editor "code --wait"
```

注意：在安装 Git 时也可以进行设置