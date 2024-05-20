Sure, here's the translation of the Chinese text into English:

```markdown
<h1 style="color: #e19cab;">How to Build a Website</h1>
<h2 style="color: #e19cab;">1. Preparation</h2>
  
We will use the following tools to build our own website:

- Git: Used for version control on GitLab. (P.S. From experience, Mac users also need to download and install it. Remember to disconnect from the internet during installation, otherwise, it might get stuck.)
- GitHub: Used as our web hosting service.
- GitHub Desktop: Facilitates transferring code from local to GitHub.
- Node.js for building environment.
- VScode for writing documents.
- Markdown language for writing our documents.
- Image upload service: We use PicGo to store our images in the cloud (for example, on GitLab) and use them in our markdown documents.

<h2 style="color: #e19cab;">2. Website Setup</h2>

<h3 style="color: #e19cab;">Creating a GitHub Repository</h3>

First, you need to create a new repository on GitHub to host your website.

1. Log in to your GitHub account.
2. Create a new public repository where you can collaborate with your team to create web content.  
    ![Image 1](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/1.png)
3. Name your repository, choose between public or private, add a README file to share information, and then click the "Create repository" button.  
    ![Image 2](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/2.png)
4. Leave the page settings empty. Click on the repository's settings, select "Pages" from the left, choose "main" and "/root", then save. The link above allows you to view the page.  
    ![Image 3](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/3.png)

<h3 style="color: #e19cab;">Inviting Team Members</h3>

1. Open the created repository.  
   ![Image 4](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/4.png)
2. Click on "Settings", find "Collaborators" on the left, then click "Add people", enter their email addresses, and set their roles (maintainer).  
   ![Image 5](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/5.png)  
   ![Image 6](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/6.png)

<h3 style="color: #e19cab;">Uploading to the Web</h3>

Clone the repository to GitHub.

1. Click "Add", "Clone repository", find the repository you want to clone, and finally click "Clone".  
   ![Image 7](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/7.png)  
   ![Image 8](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/8.png)

<h3 style="color: #e19cab;">GitHub Desktop Login</h3>

1. Find your repository, click on "Open in Visual Studio Code", input new content in Visual Studio Code, and save.  
   ![Image 9](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/9.png)
2. After document changes, input anything in the first box, then click "Commit to main", and then "Push origin". If the icon shows a loop, the sync is successful.  
   ![Image 10](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/10.png)  
   ![Image 11](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/11.png)

<h2 style="color: #e19cab;">How to Deploy and Analyze a Docsify Document Website</h2>
Docsify is a lightweight documentation website generation tool that allows you to quickly build interactive documentation websites. Below is a brief tutorial on how to deploy and analyze a document website using Docsify.

<h3 style="color: #e19cab;">1. Preparation:</h3>
Ensure that Node.js and npm are installed on your computer. You can check if they are installed by running the following commands in the terminal (open VScode, open a new terminal) or command prompt:

   `node -v`
   `npm -v`

   ![Image 12](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/12.png)

   If not installed, you can download and install them from the official Node.js website: https://nodejs.org/

   Open settings, find developer settings, click on Tokens (classic), select "generate new token" (classic), then enter a name in the note, change the expiration as desired, select repo, workflow, write: packages, and generate the token, then copy it.

<h3 style="color: #e19cab;">2. Installing Docsify</h3>

1. Install Docsify: Enter the following code  
   `npm i docsify-cli -g`
   ![Image 19](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/blob/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/19.png)

2.<h3 style="color: #e19cab;">2. Installing Docsify (continued)</h3>

2. Determine the location, then initialize the environment: Enter the following code, and input 'y' when prompted in the yellow box  
   `docsify init ./docs`
   ![Image 20](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/blob/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/20.png)

3. Preview:  
   `docsify serve docs`
4. Browser access: http://localhost:3000
   ![Image 21](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/blob/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/21.jpg)

<h3 style="color: #e19cab;">3. Creating Website Cover Page:</h3>

1. Create a new folder to store your Docsify project and create an HTML file named index.html in that folder. In Visual Studio Code, select "File" > "New File" > "HTML File" as the file type and name the file.

   ![Image 22](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/blob/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/22.png)

2. Write configuration and content: In the newly created HTML file, write the basic structure of the webpage, including <html>, <head>, and <body> tags. Inside the <body> tag, write the content of the website cover, including title, slogan, background image or video, etc.

   ![Image 23](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/blob/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/23.jpg)

3. Add CSS styles: Inside the <head> tag, use <style> tags or link external CSS files to add styles to the website cover, including adjusting the size of background images, text colors, and sizes, etc.

4. Test and debug: After saving the file, open it in a browser to view the effect of the website cover, and make necessary debugging and modifications until the desired effect is achieved.

<h3 style="color: #e19cab;">4. Setting Up Cover Page:</h3>

1. Create a cover page file.

   ![Image 24](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/blob/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/24.jpg)

<h3 style="color: #e19cab;">5. Creating Sidebar:</h3>

1. Add a sidebar container to the website cover: In the HTML structure of the website cover, add a <div> or other container element as the sidebar container.

2. Write sidebar content: Inside the sidebar container, write the content of the sidebar, including navigation links, search boxes, personal profiles or information, etc.

   ![Image 25](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/blob/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/25.png)

3. Add CSS styles to the sidebar: Use CSS styles to add styles to the sidebar container and its content, including setting background colors, border styles, text styles, etc.

4. Test and debug: After saving the file, view the website cover and sidebar effects in the browser to ensure they are displayed correctly and responsive on different devices.

<h2 style="color: #e19cab;">5. Deploying to GitHub Pages (Optional):</h2>

If you want to deploy the documentation website to GitHub Pages, you can push the Docsify project to a GitHub repository and enable the GitHub Pages feature.

<h3 style="color: #e19cab;">Image Upload:</h3>

1. Install PicGo.
2. Create a new image repository on GitHub.
3. Access the image bed settings.
4. Get the key.
5. Set up a custom domain using CDN acceleration: https://cdn.jsdelivr.net/gh/username/repositoryname.
6. Click on image bed settings, find GitHub, paste the key into the token, and fill in the rest as required.

   ![Image 13](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/13.png)
   ![Image 14](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/14.png)
   ![Image 15](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/15.png)

7. Drag and drop the images to the upload area, check if they are uploaded successfully in the album, and you can also copy the image path.

   ![Image 17](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/17.png)
   ![Image 18](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/18.png)
   (P.S. If the PicGo configuration fails continuously, you can directly create a folder named 'images' in the GitHub repository to store the images and add them.)

