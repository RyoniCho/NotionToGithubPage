# NotionToGithubPage

## 1. Notion To Github page?

Python script that converts pages created in Notion to the format of the GitHub Pages-based (jekyll) blog. 
It was created by referring to [Uonway's Project](https://github.com/uoneway/Notion-to-GitHub-Pages). Thank you.

## 2. Function

- Convert the markup file and image folder exported from Notion to match the post format of the Jekyll service in GitHub Pages.

  - It makes the Image files in image folder move to *assets/images/posts/{Input Title}* folder.
  - The image path in the markdown file will also be modified accordingly.
  - Markdown file rename  *date-{inputted title}.md*.
  - Front matter is reflected in the markdown file for contents written in the custom text file. 

  

## 3. How to Use

1. Python 3.x version installation is required. 

2. Download the ***notionToGithubPage.py*** file and ***customFrontMatter.txt** and move it to the GitHub Pages root folder on your local PC ( *GitHub Pages root*).

3. Export the Notion notes you want to upload to GitHub Pages from the Notion app in *Markdown & CSV* format.

4. Move the zip file exported from Notion to the *GitHub Pages root* path on your local PC.

5. Open the ***customFrontMatter.txt** file to modify the Front Matter information on that post (it does not include the title and date).

6. On the Local computer, go to the *GitHub Pages root* path in the Shell, then type:

       python motionToGithubPagePy

7. Enter title and date information.

8. At the end of this course, *Date-{Input Title}.md* is generated and the associated image files are moved to  *assets/images/posts/{Input Title}* folder. Please move only the md file to the desired location in the *_post*  folder.

## 4. Notice

- This Script only tested in Mac OS Platform. 

  

Feedback and enquiries, forks are always welcome :)
