# developik-um.github.io

# Jenkins Resume Creation

## Purpose  
Primary goal of the following readme document is to explain detailed steps of how to create a resume using  
Jenkins static website generator and host it on Github pages.


## Getting Started

These instructions will give you a copy of the project up and running on
your local machine for development and testing purposes. See deployment
for notes on deploying the project on a live system.

### Prerequisites

OS:
- Windows 10  

Requirements for the software and other tools to build, test and push :
- Install [Ruby Development Kit]() 
- Install [Git Bash](), that recommended command line if you want to closely follow tutorial in this readme document

- [Example 1](https://www.example.com)
- [Example 2](https://www.example.com)

### Installing

A step by step series of examples that tell you how to get a development
environment running

Say what the step will be

    Give the example

And repeat

    until finished

End with an example of getting some data out of the system or using it
for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Sample Tests

Explain what these tests test and why

    Give an example

### Style test

Checks if the best practices and the right coding style has been used.

    Give an example

## Deployment

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
    git -b checkout gh-pages
```
  - Type the following commands to add all files, commit and push them your repository
```
    git add .
    git -m commit "your commit message"
    git push 
```
- Type in your password and username or set up ssh connection between your local machine and github account to proceed
- 


## Built With

  - [Contributor Covenant](https://www.contributor-covenant.org/) - Used
    for the Code of Conduct
  - [Creative Commons](https://creativecommons.org/) - Used to choose
    the license

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code
of conduct, and the process for submitting pull requests to us.

## Versioning

We use [Semantic Versioning](http://semver.org/) for versioning. For the versions
available, see the [tags on this
repository](https://github.com/PurpleBooth/a-good-readme-template/tags).

## Authors

  - **Andrii Provozin** - *Provided README Template* -
    [developik](https://github.com/developik)  
    [developik-um](https://github.com/developik-um)  

## License

This project is licensed under the [MIT License](LICENSE) - see the [LICENSE](LICENSE) file for details

## Acknowledgments  
<b>Thanks to:</b>  
  - [Mike Dane](https://www.youtube.com/channel/UCvmINlrza7JHB1zkIOuXEbw) for a great Jenkins introduction tutorial
  - Stewart Wilcox for teaching course Comp 3040
  - My group members for the review of this document
  - [PurpleBooth](https://github.com/PurpleBooth/) for template example 
  - And anyone related to creating Jenkins static website generator

## FAQ  
  
- “Why is Markdown better than a word processor?”  
  - Answer 1
- “Why is my resume not showing up?"
  - Answer 2
