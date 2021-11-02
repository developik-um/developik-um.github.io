## Creating and hosting simple Jenkins Static Website on Github pages

### Purpose  
<i>Primary goal of the following readme document is to explain detailed steps of how to create a resume using  
Jenkins static website generator, host it on Github pages and explain how to follow Etter’s protocol.</i>  

> If documentation is not publicly available Wiki where every change should be immidiately syncronized, then it is best to have a static documentation.
> It weighs less, easier to manage and less complicated overall.

### Our stack
- Markdown
- Markdown editor
- GitHub Pages
- Jekyll

### Prerequisites  
<i>Make sure to have the following prerequisites to start with the tutorial.</i>

OS:
- Windows 10  

Other required software and tools:  
- Install [Ruby Development Kit]() 
- Install [Git Bash](), that recommended command line if you want to closely follow tutorial in this readme document  
- Create an account on an online markdown editor [Stackedit](https://stackedit.io/)

### Creating Resume  
<i> Steps for moving your resume to markdown format </i>  
- Go to a markdown editor page [Stackedit - Markdown page](https://stackedit.io/app)
- Copy your resume from your word or text document to a text box on this page
- Make corrections to make it look as similar as possible to your formated resume using markdown techniques. Refer to markdown tutorial in [More Resources](#more-resources) section for more information about useful techniques for formatting your markdown file.
- After you done formatting your resume, download it by doing the following steps:
    - Click <b>"Toggle side bar"</b>
    - Click <b>"Import/Export"</b>
    - Click <b>"Export as Markdown file"</b>

> Empahasis on what is important was completed according to styling recommendations by A.Ether.

![Gif Actions](https://github.com/developik-um/developik-um.github.io/blob/gh-pages/assets/Animation1.gif)  

After download is complete save that file and keep it until we come back to it a bit later.

### Installing  

<i>A step by step series of examples that tell you how to get a development
environment running.</i>

Make sure that Ruby Development Kit is installed by running the following command in the terminal:
```
ruby -v
```

You should now see the Ruby's version as an output.  
If that is not the case then try to re-install ruby development kit again.  

Next step for you will be to install gem bundler by running the following command on the next line:

```
gem install bundler jekyll
```  

For any question or issues that occured during running this bundler refer to their [documentation](https://bundler.io/).

It will take some time to complete, after it's complete you should see the following message:  

![message_1](https://github.com/developik-um/developik-um.github.io/blob/gh-pages/assets/message_1.png)  

> Content should look pleasant and easy to scan, so including images and gif's are a great way to increase reader's attention.  

Now, make sure that gem bundle is installed by pasting the following command into the terminal:

```
gem -v
```

If everything went smoothly so far we could get started with building jekyll static website.

### Building Website  
<i> How to create and build your website using Jenkins static website builder.</i>  
Create and locate the folder where you are planning to create your website using

```
cd "path/folder name"
```

Then run the following command to create jekyll project:  

```
jekyll new your-blog
```

Where 'your-blog' is the name of your project.  

Then go into recently created project:  
```
cd your-blog
```

And run command to start server for making changes and building your static website:

```
bundle exec jekyll serve
```  

Now paste in the resume that you created in the section [Creating Resume](#creating-resume) into index.md file and change front matter block from Home to a regular page.  
The following Yaml configuration will work as of now:  

```
---
layout: page
title: Resume
---
```  

Now remove any other files with markdown format from the main folder. You should now have the page with only your resume on the home page.  
To check whether it displays correctly locally access the link displayed in the terminal.  

![message_2](https://github.com/developik-um/developik-um.github.io/blob/gh-pages/assets/message_2.png) 

![Gif Actions](https://github.com/developik-um/developik-um.github.io/blob/gh-pages/assets/Animation2.gif) 

If you want to make your resume looks more stylish make sure to check out small free course by Mike Dane on youtube. 
[Link to the course](https://www.youtube.com/watch?v=pxua_1vyFck&list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB&index=4)  

After you confirm that everything looks as you would want it to be it is time for deployment to Github pages.


### Deployment  

After website is complete and you are ready to host make sure to complete the following steps.

- Build Jenkins website:
```
    bundle exec jekyll serve
```    
- Host it on Github pages:
  - Register on website [Github](github.com) and go into your account
  - Create a new repository, and once you are on the main page of the repository press copy button and copy https link
  - Go into your terminal and change current directory to the folder with your project 

Note: Make sure that the name of the your repository corresponds to the following pattern "your_username.github.io"  

> Andrew Ether recommends using distributed version control like git so that is what I'm using in this tutorial as well.  

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

Your resume should be now publicly available for everyone on "https://your_username.github.io" within two minutes.  

> Key characteristics of a good documentation are discoverability, searchability and only relevant information.
> Hence, we should stop here and let reader enjoy what they created while following this tutorial.

Congratulations on completing this tutorial!  

### Authors

  - **Andrii Provozin** - *Provided this README and Jekyll website*  
        - [developik](https://github.com/developik)  
        - [developik-um](https://github.com/developik-um)  

### License

This project is licensed under the [MIT License](LICENSE) - see the [LICENSE](LICENSE) file for details.  

> Legal issues could be a problem as mentioned in the book "Modern Technical Writing" by A.Ether.
> Hence, including license is important to reduce possibility of legal problems.

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
  
- "Why is Markdown better than a word processor?"  
    - Markdown is better than word processor, because style could be kept when moving from one editor to another. And the document will look the same on all editors that support FGM (Flavour Github Markdown). 
- "Why is my resume not showing up?"
    - There are number of reasons, but I would recommend uninstalling all software that was installed during this tutorial and try to start from the beginning of the tutorial again.
- "Why markdown styling hasn't been applied?"
    - Try to look for any extra spaces or invisible character in your markdown file which might disrupt the look of a specific line of paragraph.
