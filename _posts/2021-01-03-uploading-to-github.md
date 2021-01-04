---
published: false
---
## Uploading existing folders to Github as a repo

**1. If on windows open gitbash and browse to the folder you want to upload**

**2. create a new repository on github.com**

**3. Initialize the repo**
```
git init
```

**4. If you don't have a README.md file, create one**
```
touch README.md
```

**5. Prepare to add all the files from my folder to the git repo on your laptop**

```
git add .
```

**6. Commit the folder to the repo**

```
git commit -m "completed final project for cisw327"
```

**7. point the git repo on your laptop to the git repo in the cloud and give it a nick name 'origin'**

```
git remote add origin https://github.com/eshanis/html-css-site.git
```

**8. Finally upload ('push' command) the git repo to the cloud **

```
git push -u origin master
```

**9. Check on your github.com that the repo is updated **

**10. If you want, convert the repo into github hosted web page by going into setting and enable github page**






Enter text in [Markdown](http://daringfireball.net/projects/markdown/). Use the toolbar above, or click the **?** button for formatting help.
