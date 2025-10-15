# MD Blog

This is a single-file, client-side blog application designed to display blog posts written in Markdown. It uses plain HTML, CSS, and JavaScript, relying on the blog.txt and posts.txt files for configuration, making it incredibly easy to manage without editing any code.

## How to Run

Ensure you have the following files in the same directory:

index.html (The main application file)

blog.txt (For site title and subtitle)

posts.txt (For the list of posts)

Open index.html directly in any modern web browser (Chrome, Firefox, Edge, etc.).

## How to Configure Your Blog

All configuration is done via two simple text files.

1. Setting the Header (blog.txt)
This file controls the main Title and Subtitle displayed on the homepage.

Line

Content

Purpose

Line 1

My MD Text Blog

The main <h1> title of the blog.

Line 2

A simple, text-configured Markdown blog.

The subtitle displayed below the title.

To change your blog's name, simply edit the first two lines of blog.txt.

2. Managing Your Posts (posts.txt)
This file determines which posts appear on the homepage and their order. The application reads each line and parses it using the pipe (|) character as a separator.

Format:

[Filename] | [Title] | [Description]

How to Add a New Post:
Create your content file: Write your post content in a new Markdown file (e.g., new-post.md).

Open posts.txt.

Add a new line following the required format:

my-new-post.md | My Awesome New Post Title | A brief summary of what this post covers.

The new post will automatically appear on the blog's homepage when you refresh index.html.

Field Details
Field

Requirement

Notes

Filename

Required. Must end in .md.

This file must exist in the same directory.

Title

Optional

If left blank, the script will use the filename (cleaned up) as the title.

Description

Optional

This text appears as a short snippet under the title on the list view.

Example of the selected Canvas content:

Note: Lines starting with the # character are treated as comments and are ignored by the application, so feel free to use them for organization or notes.
