<h1 style="color: #e19cab;">怎样建设一个网站</h1>
<h2 style="color: #e19cab;">1. 准备</h2>
  
我们将使用以下工具来构建我们自己的网页：

- Git：用于控制我们在GitLab中的版本。（ps. 经验所言，Mac也是需要下载并安装的哦，同时在安装时，记得断网，不然会卡住的。)
- 使用GitHub作为我们网页的服务。
- GitHub桌面：方便我们将编码从本地传输到GitHub。
- 使用Node.js构建环境。
- 用于写文档的VScode。
- 撰写我们文档的Markdown语言。
- 图片上传服务，我们使用PicGo将我们的图片存储在云端（例如在GitLab），并在标记文档中使用。

<h2 style="color: #e19cab;">2. 网页设置</h2>

<h3 style="color: #e19cab;">创建GitHub存储库</h3>

首先，你需要在GitHub上创建一个新的存储库来托管你的网站。

1. 登录你的GitHub账号。
2. 创建一个公共存储库，然后您可以与您的团队一起创建web内容。  
    ![图片1]（https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/1.png）
3. 给您的存储库命名，选择公共或私有。添加一个README文件来共享您的信息，然后单击“create repository”按钮。  
    ![图片2](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/2.png)
4. 设置页面为空。单击存储库的设置，并选择左侧的“page”。选择“main”和“/root”并保存。上面的链接允许您查看该页。  
    ![图片3](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/3.png)

<h3 style="color: #e19cab;">邀请团队成员</h3>

1. 打开创建的存储库。    
   ![图片4](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/4.png)
2. 单击“设置”，在左侧找到“协作者”，然后单击“添加人员”，输入他们的电子邮件地址并设置他们的身份（maintain）。  
   ![图片5](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/5.png)  
   ![图片6](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/6.png)

<h3 style="color: #e19cab;">网络上传</h3>

将存储库克隆到GitHub。

1. 点击“添加”，“克隆资源”，找到需要克隆的存储库。最后按一下克隆。  
   ![图片7](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/7.png)  
   ![图片8](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/8.png)

<h3 style="color: #e19cab;">Github桌面登录</h3>

1. 找到您的存储库，单击打开“在Visual Studio Code中打开”，在Visual Studio Code中输入新内容并保存。  
   ![图片9](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/9.png)
2. 文档更改后，在第一个框中输入任何内容，然后单击Commit to main，然后push origin，如果图标显示为循环，则同步成功。  
   ![图片10](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/10.png)  
   ![图片11](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/11.png)

<h2 style="color: #e19cab;">如何部署并分析 Docsify 文档网站</h2>
Docsify 是一个轻量级的文档网站生成工具，使用它可以快速构建具有交互性的文档网站。下面是一份简要的教程，介绍如何使用 Docsify 部署并分析文档网站。
<h3 style="color: #e19cab;">1.准备工作：</h3>
确保你的电脑上已经安装了 Node.js 和 npm。你可以在终端（打开VScode，新建终端
）或命令提示符中运行以下命令来检查是否安装：

   `node -v`
   `npm -v`

![图片12](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/12.png)
如果未安装，你可以从 Node.js 的官方网站下载并安装：https://nodejs.org/

点开setting，找到developer setting，点击Tokens（classic）选择generate new token（classic）再在note中输入名称，将expiration改成想要的时间，然后将repo，workflow，write：packages全选上，生成密钥，然后复制。

<h3 style="color: #e19cab;">2.安装docsify</h3>


1. 安装docsify：输入以下代码  
   `npm i docsify-cli -g`
![图片19](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/19.png)

2. 确定位置，然后初始化环境：输入以下代码后，在黄色框处输入y
   `docsify init ./docs`
![图片20](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/20.png)

3. 预览：  
   `docsify serve docs`
4. 浏览器访问：http://localhost:3000
![图片21](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/21.jpg）


<h3 style="color: #e19cab;">3.创建网页封面：</h3>

1.创建一个新的文件夹来存放你的 Docsify 项目，并在该文件夹中创建一个名为 index.html 的 HTML 文件。在 Visual Studio 中，选择“文件” > “新建” > “文件”，选择“HTML 文件”作为文件类型，并为文件命名。

![图片22](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/22.png）

2. 编写配置和内容：在新建的 HTML 文件中编写网页的基本结构，包括 <html>、<head> 和 <body> 标签。在 <body> 标签内部，编写网页封面的内容，包括标题、标语、背景图片或视频等。
![图片22](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/24.jpg）

3.   添加 CSS 样式：在 <head> 标签内部，使用 <style> 标签或链接外部 CSS 文件，为网页封面添加样式，包括调整背景图片的大小、文字的颜色和大小等。
4.测试和调试：保存文件后，在浏览器中打开 HTML 文件，查看网页封面的效果，并进行必要的调试和修改，直到达到预期的效果。

<h3 style="color: #e19cab;">4.设置cover page</h3>

1.建立一个cover page 文件

![图片22](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/25.png）

<h3 style="color: #e19cab;">5.建立sidebar：</h3>
1.在网页封面中添加侧边栏容器：在网页封面的 HTML 结构中，添加一个 <div> 或其他容器元素，作为侧边栏的容器。
2.编写侧边栏内容：在侧边栏容器内部，编写侧边栏的内容，包括导航链接、搜索框、个人资料或信息等。

![图片22](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/26.png）

3.为侧边栏添加 CSS 样式：使用 CSS 样式为侧边栏容器和其中的内容添加样式，包括设置背景颜色、边框样式、文字样式等。
4.测试和调试：保存文件后，在浏览器中查看网页封面和侧边栏的效果，确保它们在不同设备上都能够正确显示和响应。

<h2 style="color: #e19cab;">5. 部署到 GitHub Pages（可选）：</h2>
如果你希望将文档网站部署到 GitHub Pages 上，可以将 Docsify 项目推送到 GitHub 仓库，并启用 GitHub Pages 功能。




<h3 style="color: #e19cab;">图片上传</h3>

1. 安装Picgo
2. 在GitHub上新建图片仓库
3. 进入图床设置
4. 获取密钥
5. 设定自定义域名使用cdn加速https://cdn.jsdelivr.net/gh/用户名/图床仓库名，完成Picgo设置  
   ![图片13](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/13.png)  
   ![图片14](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/14.png)  
   ![图片15](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/15.png)
6. 点击图床设置，找到GitHub，将密钥复制到token上，其他的按要求填完。  
   ![图片16](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/16.png)
7. 接着将图片拖拽到上传区，在相册中查看是否上传成功，同时可以复制图片路径  
   ![图片17](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/17.png)  
   ![图片18](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/18.png)
   (ps. 如果picgo配置一直失败，可以直接在Github仓库中创建存放images的文件夹，并Add file。)