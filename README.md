# developik-um.github.io

# Jenkins Resume Creation  

### Purpose  
Primary goal of the following readme document is to explain detailed steps of how to create a resume using  
Jenkins static website generator and host it on Github pages.

### Prerequisites  
Make sure to have the following prerequisites to start with the tutorial.  

OS:
- Windows 10  

Requirements for the software and other tools to build, test and push:  
- Install [Ruby Development Kit]() 
- Install [Git Bash](), that recommended command line if you want to closely follow tutorial in this readme document  

### Installing  

A step by step series of examples that tell you how to get a development
environment running  

Say what the step will be

    Give the example

And repeat

    until finished

End with an example of getting some data out of the system or using it
for a little demo  

### Deployment  

After website is complete and you are ready to host make sure to complete the following steps.

- Build Jenkins website:
```
    bundle exec jekyll serve
```    
- Host it on Github pages:
  - Register on website [Github](github.com) and go into your account
  - Create a new repository, and once you are on the main page of the repository press copy button and copy https link
  - Go into your terminal and locate folder with your project

```
  - Go into you project directory and type the following if you haven't initialized the project yet
```
    git init
```
  - Connect project on your local device to your repository by running the following command, but replace "github.com/username/your-repo.git" with the link that you copied in the previous steps
```
    git remote add origin github.com/username/your-repo.git
```
  - Create and switch to the branch "gh-pages" by running the following command:
```
    git checkout -b gh-pages
```
  - Type the following commands to add all files, commit and push them your repository
```
    git add .
    git -m commit "your commit message"
    git push origin gh-pages
```
- Type in your password and username or set up ssh connection between your local machine and github account to proceed
- If you get an error saying that branch can't be pushed try running the following command instead
```
    git push --set-upstream origin gh-pages
```

### Versioning

We use [Semantic Versioning](http://semver.org/) for versioning. For the versions
available, see the [tags on this
repository](https://github.com/PurpleBooth/a-good-readme-template/tags).

### Authors

  - **Andrii Provozin** - *Provided README Template* -
    [developik](https://github.com/developik)  
    [developik-um](https://github.com/developik-um)  

### License

This project is licensed under the [MIT License](LICENSE) - see the [LICENSE](LICENSE) file for details

### Acknowledgments  
<b>Thanks to:</b>  
  - [Mike Dane](https://www.youtube.com/channel/UCvmINlrza7JHB1zkIOuXEbw) for a great Jenkins introduction tutorial
  - Stewart Wilcox for teaching course Comp 3040
  - My group members for the review of this document
  - [PurpleBooth](https://github.com/PurpleBooth/) for template example 
  - And anyone related to creating Jenkins static website generator

### More Resources
- [Markdown tutorial](https://www.markdownguide.org/getting-started/)
- [Etter’s book](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
- [Make a Readme website](https://www.makeareadme.com/)
- [Markdown Tutorial](https://www.markdowntutorial.com/)

### FAQ  
  
- “Why is Markdown better than a word processor?”  
  - Answer 1
- “Why is my resume not showing up?"
  - Answer 2
