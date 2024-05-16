<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>My Docsify Site</title>
  <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
  <meta name="description" content="Description">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0">
  <link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify@4/lib/themes/vue.css">
</head>
<body style="background: linear-gradient(to bottom, #E6E6FA, #9370DB);"> <!-- 浅紫色渐变背景色 -->
  <div id="app"></div>
  <script>
    window.$docsify = {
      name: 'zju-fab',
      repo: '', // 将仓库链接或留空
      loadSidebar: true,
      loadNavbar: true,
      coverpage: '_coverpage.md', // 指定封面页文件
      subMaxLevel: 3,
      homepage: 'README.md', // 指定主页文件
    }
  </script>
  <!-- Docsify v4 -->
  <script src="//cdn.jsdelivr.net/npm/docsify@4"></script>
</body>
</html>
