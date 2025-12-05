# MD Blog

MD Blog is a single-file, client-side blog application designed to display blog posts written in Markdown. It uses plain HTML, CSS, and JavaScript, relying on the blog.txt and posts.txt files for configuration, making it incredibly easy to manage without editing any code.

## How to Run
Download the MD Blog source files from [Github.com](https://github.com/barneyme/mdblog/).

Ensure you have the following files in the same directory on your web server:

* **index.html** (The main application file)
**blog.txt** (For site title and subtitle)
**posts.txt** (For the list of posts)
Open index.html directly from any web server in any modern web browser (Chrome, Firefox, Edge, etc.).&nbsp;
([XAMPP](https://www.apachefriends.org/download.html) is great local web server.)

## How to Configure Your Blog
All configuration is done via two simple text files.

**blog.txt**
This file controls the main Title and Subtitle displayed on the homepage.
Line 1 is the main title of the blog.
Line 2 is the subtitle displayed below the title.

To change your blog's name, simply edit the first two lines of blog.txt.

**posts.txt**
This file determines which posts appear on the homepage and their order. The application reads each line and parses it using the pipe (|) character as a separator.
Format:
[Filename] | [Title] | [Description]

# **How to Add a New Post**
Each new post is&nbsp;a new Markdown file (e.g., new-post.md). (Use mdedit.html or any Markdown compatible editor.)Save your new post as a .MD file.Open posts.txt.&nbsp;Add a new line following the required format: new-post.md | My New Post Title | A brief summary of what this post covers.Upload your new posts .MD file to your web server.The new post will automatically appear on the blog's homepage when you refresh index.html.