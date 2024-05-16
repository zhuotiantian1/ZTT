# 建设网站教程

## 1. 准备

我们将使用以下工具来构建我们自己的网页：

- Git：用于控制我们在 GitLab 中的版本，mac 不需要安装，它用于设置 Git 和 GitLab。
- GitHub 作为我们网页的服务。
- GitHub 桌面：方便我们将编码从本地传输到 GitHub。
- 使用 Node.js 构建环境。
- 用于写文档的 VScode。
- 撰写我们文档的 Markdown 语言。
- 图片上传服务，我们使用 PicGo 将我们的图片存储在云端（例如在 GitLab），并在标记文档中使用。

## 2. 网页设置

### 创建 GitHub 存储库

首先，你需要在 GitHub 上创建一个新的存储库来托管你的网站。

1. 登录你的 GitHub 账号。
2. 创建一个公共存储库，然后您可以与您的团队一起创建 web 内容。
![图片1](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/a876c079a624d3ce907da503803aa2150b97cf8d/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/1.png)

3. 给您的存储库命名，选择公共或私有。添加一个 README 文件来共享您的信息，然后单击“create repository”按钮。
![图片2](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/a876c079a624d3ce907da503803aa2150b97cf8d/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/2.png)

4. 设置页面为空。单击存储库的设置，并选择左侧的“page”。选择“main”和“/root”并保存。上面的链接允许您查看该页。
![图片3](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/a876c079a624d3ce907da503803aa2150b97cf8d/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/3.png)

### 邀请团队成员

1. 打开创建的存储库。
![图片4](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/4.png)

2. 单击“设置”，在左侧找到“协作者”，然后单击“添加人员”，输入他们的电子邮件地址并设置他们的身份（maintain）。

### 网络上传

将存储库克隆到 GitHub。

1. 点击“添加”，“克隆资源”，找到需要克隆的存储库。最后按一下克隆。

### Github 桌面登录

1. 找到您的存储库，单击打开“在 Visual Studio Code 中打开”，在 Visual Studio Code 中输入新内容并保存。
2. 文档更改后，在第一个框中输入任何内容，然后单击 Commit to main，然后 push origin，如果图标显示为循环，则同步成功。

### Docsify

打开 VScode，新建终端。

1. 安装 docsify：`npm i docsify-cli -g`
2. 确定位置，然后初始化环境：`docsify init ./docs`
3. 预览：`docsify serve docs`
4. 浏览器访问：[http://localhost:3000](http://localhost:3000)

### 图片上传

1. 安装 Picgo
2. 在 GitHub 上新建图片仓库
3. 进入图床设置
4. 获取密钥
5. 设定自定义域名使用 cdn 加速 [https://cdn.jsdelivr.net/gh/用户名/图床仓库名](https://cdn.jsdelivr.net/gh/用户名/图床仓库名)，完成 Picgo 设置
6. 点击图床设置，找到 GitHub，将密钥复制到 token 上，其他的按要求填完。
