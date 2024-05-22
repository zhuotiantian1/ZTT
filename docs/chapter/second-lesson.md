<h1 style="color: #e19cab;">How to Build a Website</h1>
<h2 style="color: #e19cab;">1. Preparation</h2>
  
We will use the following tools to construct our own web page:

- Git: Used to control versions of our code in GitLab. (PS. Based on experience, Mac users also need to download and install it. Remember to disconnect from the internet during installation, or it might get stuck.)
- GitHub: Serving as our web page hosting service.
- GitHub Desktop: Facilitating the transfer of our code from local to GitHub.
- Node.js for building environment.
- VScode for document writing.
- Markdown language for writing our documents.
- Image upload service: We use PicGo to store our images in the cloud (e.g., on GitLab) and use them in our markup documents.

<h2 style="color: #e19cab;">2. Web Page Setup</h2>

<h3 style="color: #e19cab;">Creating GitHub Repository</h3>

Firstly, you need to create a new repository on GitHub to host your website.

1. Log in to your GitHub account.
2. Create a public repository where you can collaborate with your team to create web content.

![图片1]（https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/1.png）

3. Name your repository, choose whether it's public or private. Add a README file to share your information, then click the "create repository" button.

    ![图片2](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/2.png)
4. 
Set the page to be empty. Click on the settings of the repository and select "Pages" on the left. Choose "main" and "/root" and save. The link above allows you to view the page.
    ![图片3](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/3.png)


<h3 style="color: #e19cab;">Invite Team Members</h3>

1. Open the created repository.
   ![图片4](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/4.png)

2. Click on "Settings", find "Collaborators" on the left, then click "Add people", enter their email addresses, and set their role (maintainer). 
   
   ![图片5](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/5.png)  
   ![图片6](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/6.png)

<h3 style="color: #e19cab;">Upload to Web</h3>

Clone the repository to GitHub.

1. Click on "Add", "Clone a resource", find the repository you want to clone. Finally, click "Clone".

   ![图片7](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/7.png)  
   ![图片8](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/8.png)

<h3 style="color: #e19cab;">GitHub Desktop Login</h3>

1. Find your repository, click "Open in Visual Studio Code", input new content in Visual Studio Code, and save.

   ![图片9](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/9.png)

2. After making changes to the document, input any content in the first box, then click "Commit to main", and then "Push origin". If the icon displays a loop, synchronization is successful.

   ![图片10](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/10.png)  
   ![图片11](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/11.png)

<h2 style="color: #e19cab;">How to Deploy and Analyze Docsify Document Website</h2>
Docsify is a lightweight document website generation tool that allows you to quickly build interactive document websites. Below is a brief tutorial on how to deploy and analyze a document website using Docsify.

<h3 style="color: #e19cab;">1. Preparation:</h3>
Ensure that Node.js and npm are installed on your computer. You can run the following commands in the terminal (open VScode, open a new terminal) or command prompt to check if they are installed:

   <code>node -v</code>
   <code>npm -v</code>


![图片12](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/12.png)

If not installed, you can download and install from the official website of Node.js: [https://nodejs.org/](https://nodejs.org/)

Click on "Setting", find "Developer Setting", click on "Tokens (classic)", select "generate new token (classic)", then enter a name in the note, change the expiration to the desired time, then select "repo", "workflow", "write:packages", generate the key, and then copy it.

<h3 style="color: #e19cab;">2. Install Docsify</h3>

1. Install Docsify: Input the following code
   <code>npm i docsify-cli -g</code>

![图片19](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/19.png)

2. Determine the location, then initialize the environment: After entering the following code, input y in the yellow box.
   `docsify init ./docs`
![图片20](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/20.png)

3.Preview:  
   `docsify serve docs`
4. Access in browser:：http://localhost:3000

![图片21](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/21.jpg）

<h3 style="color: #e19cab;">3. Creating Webpage Cover:</h3>

1. Create a new folder to store your Docsify project, and within that folder, create an HTML file named index.html. In Visual Studio, select "File" > "New" > "File", choose "HTML File" as the file type, and name the file.

![图片22](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/22.png）

2. Write Configuration and Content: In the newly created HTML file, write the basic structure of the webpage, including <html>, <head>, and <body> tags. Within the <body> tag, write the content of the webpage cover, including titles, slogans, background images or videos, etc.

![图片22](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/24.jpg）

3. Add CSS Styles: Within the <head> tag, use <style> tags or link external CSS files to add styles to the webpage cover, including adjusting the size of background images, text color, and size, etc.

4. Testing and Debugging: After saving the file, open the HTML file in a browser to view the effect of the webpage cover and perform necessary debugging and modifications until the desired effect is achieved.

<h3 style="color: #e19cab;">4. Setting up the Cover Page</h3>

1. Create a cover page file.

![图片22](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/25.png）

<h3 style="color: #e19cab;">5.建立sidebar：</h3>

1. Add a Sidebar Container in the Webpage Cover: In the HTML structure of the webpage cover, add a <div> or other container element as the container for the sidebar.

2. Write Sidebar Content: Within the sidebar container, write the content of the sidebar, including navigation links, search box, personal profile or information, etc.

![图片22](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/26.png）

3. Add CSS Styles to the Sidebar: Use CSS styles to add styles to the sidebar container and its contents, including setting background color, border styles, text styles, etc.

4. Testing and Debugging: After saving the file, view the effect of the webpage cover and sidebar in a browser to ensure they display and respond correctly on different devices.

<h2 style="color: #e19cab;">5. Deploy to GitHub Pages (Optional):</h2>
If you want to deploy the document website to GitHub Pages, you can push the Docsify project to a GitHub repository and enable the GitHub Pages feature.

<h3 style="color: #e19cab;">Image Upload</h3>

1. Install PicGo.
2. Create a new image repository on GitHub.
3. Access the image bed settings.
4. Obtain the key.
5. Set the custom domain to use CDN acceleration. For example, `https://cdn.jsdelivr.net/gh/username/repository`, complete the PicGo setup.

   ![图片13](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/13.png)  

   ![图片14](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/14.png)  

   ![图片15](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/15.png)

6. 点击图床设置，找到GitHub，将密钥复制到token上，其他的按要求填完。  

   ![图片16](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/16.png)

7. 接着将图片拖拽到上传区，在相册中查看是否上传成功，同时可以复制图片路径 

   ![图片17](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/17.png)  

   ![图片18](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/18.png)
  
  (ps. If PicGo configuration keeps failing, you can directly create a folder named "images" in your GitHub repository and add files to it.)