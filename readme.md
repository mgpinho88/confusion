# Coursera Full-Stack Bootcamp
## Part 1: Bootstrap
In this lesson students are introduced to Bootstrap. We will use package.json with a lite-server to view renderings of the sample page.

### Table of Content
  * Pre-Text
  * Getting Started
  * Lite-server
  * Bootstrap
  * Font Awesome
  * Additional Dependencies  

## Pre-Text  
All dependencies for this project can be added with the following two lines:
```bash
npm install lite-server --save-dev
npm install bootstrap@4.0.0 bootstrap-social@5.1.1 font-awesome@4.7.0 jquery@3.3.1 popper.js@1.12.9 --save
```

# Getting Started
Step 1. Clone this repo onto your local desktop.<br>
Step 2. Install the dependencies from the "Pre-Text" section of this readme file. <br>
Step 3. In a bash terminal run the command ```npm start```


# Lite-server
Run the following command to install lite-server on for this project
```bash
npm install lite-server --save-dev
```
By running this command you will have installed the lite-server and created a dependency in your package.json file. Additionally you will need to add the lite-server to your start command. Below you will see in the "scripts" that a "start" is included in the object. This tells node what to do in order to start the project. By using lite-server we can make changes to the project and view the changes in real time.

```json
{
  "name": "confusion",
  "version": "1.0.0",
  "description": "<Brief description of the project>",
  "main": "index.html",
  "dependencies": {
    "lite-server": "^2.5.4"
  },
  "scripts": {
    "start": "npm run lite",
    "test": "echo \"Error: no test specified\" && exit 1",
    "lite": "lite-server"
  },
  "repository": {
    "type": "git",
    "url": "git+https://mgpinho@bitbucket.org/mgpinho/confusion.git"
  },
  "author": "<Your Name Here>",
  "license": "ISC",
  "homepage": "https://bitbucket.org/mgpinho/confusion#readme"
}
```

# Bootstrap
Bootstrap is a frontend framework that give your page style and responsiveness. To begin using bootstrap use the command:

```bash
npm install bootstrap --save
```

or you can specify the version using

```bash
npm install bootstrap@4.0.0 --save
```

To include Bootstrap use the link tag in the header of your page.
```HTML
<link rel="stylesheet" href="node_modules/bootstrap/dist/css/bootstrap.min.css">
<link rel="stylesheet" href="node_modules/bootstrap-social/bootstrap-social.css">
```


Using previous versions of Bootstrap ensure that there aren't major changes that effect the rendering of your page if a new version of Bootstrap is published.

Additionally, we are using Bootstraps [grid system](https://getbootstrap.com/docs/4.0/layout/grid/) to position elements of our page. Traditionally simply using HTML and CSS to position elements was a difficult task. With the advent of smartphones and tables the difficulty of rendering elements to smaller screens had an even larger layer of complexity. CSS helped mitigate the difficulty with flex-box. Bootstrap then implemented flex-box to build a grid system that works for all screen sizes.

Additionally with Bootstrap we included various elements such as breadcrumbs and a navbar for better navigation through our page. We also included social media icons as links to our social media accounts in the footer of the page.

# Font Awesome
[Font Awesome](https://fontawesome.com/) is a CSS library of icons that can be used in our page.

```bash
npm install font-awesome --save
```

To include Font Awesome use the link tag in the header of your page
```HTML
<link rel="stylesheet" href="node_modules/font-awesome/css/font-awesome.min.css">
```

Font Awesome has over 1,600 free icons to choose from and over 7,000 icons if you opt in the the yearly subscription. The icons can be customized to your websites needs. Browse through their documentation to find the icons you need.

# Other Dependencies
This project also uses jquery and popper.js. Jquery is a framework for JavaScript that is used by Bootstrap. In order to use the JavaScript elements of Bootstrap jquery must be included in the project. Popper.js is another popular JavaScript library that helps with positioning.
