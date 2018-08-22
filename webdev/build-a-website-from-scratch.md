---
title: Code a Website!
description: A step-by-step guide on coding your first website from scratch, Read now.
meta:
 - name: twitter:site 
   content: https://kaizenmedia.co.za/webdev/build-a-website-from-scratch.html
 - name: twitter:card 
   content: summary_large_image
 - name: twitter:title 
   content: Kaizen Media | Tutorials | Code Your First Website
 - name: twitter:description 
   content: A step-by-step guide on coding your first website from scratch, Read now.
 - name: twitter:image 
   content: https://kaizenmedia.co.za/code-website-kaizen.png
 - property: og:title 
   content: Kaizen Media | Tutorials | Code Your First Website
 - property: og:type 
   content: article 
 - property: og:url 
   content: https://kaizenmedia.co.za/webdev/build-a-website-from-scratch.html
 - property: og:image
   itemprop: image
   content: http://kaizenmedia.co.za/code-website-kaizen.png
 - property: og:image:url
   content: http://kaizenmedia.co.za/code-website-kaizen.png
 - property: og:image:secure_url
   content: https://kaizenmedia.co.za/code-website-kaizen.png
 - property: og:description 
   content: A step-by-step guide on coding your first website from scratch, Read now.
 - property: og:site_name 
   content: Kaizen Media
sidebar: auto
collapsable: true
---

<img src="https://kaizenmedia.co.za/code-website-kaizen.png"
     alt="Kaizen Media Build a Website from Scratch"
     width="100%"
     height="auto"
     style="margin: 0 auto" />

# Build a WebSite by coding it from scratch!
> Firstly I want to thank all of the people who voted on the polls on my [Instagram](https://instagram.com/eckigrams) and [Facebook](https://www.facebook.com/eckhardt.dreyer) pages. It gave me the motivation to make this post.

## Getting started

For a preview of what we're going to build, follow [this link](https://kaizenmedia.co.za/zentrader-logistics/). It's a fake company with some dummy text and images. But building it will teach you core ideas about HTML and CSS, how to write some code, how to view your rendered code and as a BONUS - how to make your website live!

## Setting up for development

HTML and CSS are both languages that are interpreted by browsers. You don't really need any special software (except your browser) to view it. So where do you write your code?

> On any plain text editor.

Yes, unlike many other languages that need to be built and run, you can simply write the code in a text editor of your choice and save it as .html and .css files.

### However...

It may be VERY tedious to do. Because the 'syntax' of your code, it's really easy to make a mistake like forgetting a space or missing a '<'.

Therefor we are going to download a special text editor. It's still just text that we're writing, but the editor will do nice things like: add color to the text, warn you when there are mistakes and even offer autocomplete.

## Dowload a code editor

> From this site [https://code.visualstudio.com/](https://code.visualstudio.com/)

After you have installed the code editor, open it up.

## An important extension

What's cool about VSCode is that it comes with many helpful extensions. Today we are going to install one called Live Server. 

<img src="https://kaizenmedia.co.za/extensions.png"
     alt="Kaizen Media Build a Website from Scratch"
     width="100%"
     height="auto"
     style="margin: 0 auto" />

Click on that icon and do a search for "Live Server", install it and then restart VScode. This will allow us to create a mock server from which the website we're building is going to be served.

## Starting the build

To get started, create a folder somewhere. Open VS code and in the left navigation click 'Open Folder' and choose that empty folder you created. If you don't see the left side-bar, just press *ctrl+b* or if you're on Mac - *cmd+b*.

## HTML basics

To get started with the project, we'll give a quick rundown on some important things about HTML. Start by left-clicking in the side-bar and creating a file called *index.html*.

::: tip
index.html is a standard name for html files. If we put them in a folder called home, then the website url will show www.website.com/home. *(Note there is no index after home)*. But if we name the file home.html and put it in the home folder, it will be www.website.com/home/home.html 
:::

### html structure

HTML or (Hypertext Markup Language) is a language that allows us to create elements on the webpage in their standard styles. The syntax always starts with a `<` and ends with a `>` and in between those two tags we put an element's name, after that we usally close the tag with `</` `>` with the same name in between. e.g.

```html
<nav></nav>
```

There are reserved element names, a lot of them. But I don't recommend you try to remember them all from scratch, rather use them as you need them. There are however a few I want to got through here:

## HTML text elements

HTML text elements can be either heading tags, paragraph tags, or special tags that style the text as bold, small or italic.

### Example #1 | Text elements
```html
<h1>Largest Heading</h1>
<h2>Second Largest Heading</h2>
<h3>Third Largest Heading</h3>
<h4>Fourth Largest Heading</h4>
<h5>Fifth Largest Heading</h5>
<h6>Sixth Largest Heading</h6>

<p>Paragraph Tag</p>

<p><small>small p tag</small></p>
<p><b>bold p tag</b></p>
<p><i>italic p tag</i></p>
```

That will look like:
<h1 style="font-family: times new roman">Largest Heading</h1>
<h2 style="font-family: times new roman">Second Largest Heading</h2>
<h3 style="font-family: times new roman">Third Largest Heading</h3>
<h4 style="font-family: times new roman">Fourth Largest Heading</h4>
<h5 style="font-family: times new roman">Fifth Largest Heading</h5>
<h6 style="font-family: times new roman">Sixth Largest Heading</h6>

<p style="font-family: times new roman">Paragraph Tag</p>

<p style="font-family: times new roman"><small>small p tag</small></p>
<p style="font-family: times new roman"><b>bold p tag</b></p>
<p style="font-family: times new roman"><i>italic p tag</i></p>



Note how each element gets it's own line, and always fills 100% width of the element that it is inside. That reminds me:

:::tip
Elements run from top to bottom by default, everything you add will be stacked on top of eachother on the page. Even if you do this: `<h1>Line One</h1><p>Line Two</p>`. It's the flow of the document. So writing html like that makes sense.
:::

> NOTE: This can be changed with css, and will see this when we start styling things.

## The DIV

Another really important element is the `div` element. It really does not display anything by itself, it adds an empty element on the page, in which we can place other tags to group them and seperate them. You'll commonly see:

```html
<div>
    <h1>hello!</h1>
</div>
```

Usually these divs are given attributes like `<div id="container"></div>`, this, in most cases is for CSS and JavaScript. Don't worry about JavaScript for now, but let's tackle CSS.

## CSS basics

I always imagine HTML as the skeleton of the page and css as the meat and skin (gruesome...). But if you look at the top example again, you'll see the font is different than to the rest of the page. It's the default font. Because it has no CSS applied.

### How to write CSS

CSS can be written either on the html element, in `<style></style>` tags or in a seperate file and included. (You'll see this when we start building the site).

CSS Looks something like this:

```html
<!-- On the element itself -->
<div style="font-family: sans-serif"></div>

<!-- In style tags -->
<style>
    div {
        font-family: sans-serif;
    }
</style>
```
It's rare to add styles to the element itself, because when we do that it only styles that one specific element. When we write it in style tags everything before the curly brace is the `selector` and inside the braces we have `property: value;`. Where the property is a keyword built into css, you can see all of them on: [CSS Tricks](https://css-tricks.com/). But we'll cover many in the tutorial. 

## Building the website!

Now that you have a very short, vague understanding of HTML and CSS, I'll start building the site and take you through it step-by-step. Here you'll learn by example, I find that much more fun! 
___

## Setting up the html file

Every HTML file starts like this:


```HTML
<!DOCTYPE html>
    <html>
        <head>

        </head>
    <body>

    </body>
</html>
```
This is STANDARD. All files should begin like this and here's why:

| Element                  | Description                                  |
| ------------------------ |:-------------------------------------------: |
| `<!DOCTYPE html>`        | Tells the browser this is an html file!      | 
| `<html>`                 | Indicates the start of the html              |
| `<head>`                 | Doesn't show anything on the page, but       |
|                          | adds helpful information like the title,     |
|                          | description and also where we import files   | 
| `<body>`                 | Where all the content you write is displayed | 

## Our sites Basic details

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8" />
    <meta name="title" content="ZenTraders Logistics">
    <meta name="description" content="Making sure your goods are delivered. Always.">
    <link rel="shortcut icon" href="./public/logo.png">
    <title>ZenTrader Logistics</title>
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>
<body>

</body>
</html>
```

This won't display anything on the page, but it does add the icon and title on top of the page. To see it, you'll need
to add two things in your side-bar, a new file called `style.css` which imports the css with the `<link rel="stylesheet" type="text/css" media="screen" href="style.css" />` in your head. And also a logo.png file. download any small png and drag it into your side-bar in the same folder as your index.html.

> Notice how this tag doesn't have a closing tag, it's self closing. There are more tags like this, I'll note them as they occur.

## Looking at your site

Remember the live server extension, we'll use that now. Left click in your code and select 'Open With Live Server'. This should automatically open your site in your default browser. If you've added your logo.png and our basic text you should see it in the tab on top of your browser. You're file structure in the side-bar should look like this.

```
- MainFolder
|-- index.html
|-- style.css
|-- logo.png
```

:::tip
If your site doesn't open automatically, go to your browser and type http://localhost:5500 in the url bar.
:::

## Testing if it's working
If you see your title and icon on top, you are okay, but just to be sure add this tag:

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8" />
    <meta name="title" content="ZenTraders Logistics">
    <meta name="description" content="Making sure your goods are delivered. Always.">
    <link rel="shortcut icon" href="./public/logo.png">
    <title>ZenTrader Logistics</title>
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>
<body>

    <h1>Hello World!</h1>

</body>
</html>

```

You should see this: 

<h1 style="font-family: times new roman;">Hello World!</h1>
<br>
<br>
<br>
<br>


**Woohoo! your first page!**

## First CSS

Let's clean up the font, it's ugly!

in your style.css file add this:

```css
body, html {
    margin: 0;
    padding: 0;
    font-family: sans-serif;
}
```

The margin and padding remove the automatic spacing in the file. The difference between them is that margin adds space outside and padding adds inner-space.

### Your page should look like this
___

<h1 style="font-family: sans-serif">Hello World!</h1>

___

*If it doesn't make sure to check your head file that the css is correctly imported.*

## Navbar

Let's add the navbar, it will look like this:

<section id="navbar-section">
        <nav>
            <img height="60px" id="logo" src="/website-tut-1/logo.png" alt="myLogo">
            <ul id="menu">
                <li class="menu-item"><a href="/">Home</a></li>
                <li class="menu-item"><a href="#about-section">About us</a></li>
            </ul>
        </nav>
</section>

<style>
#navbar-section {
    width: 100%;
    overflow: hidden;
}

#navbar-section nav {
    display: flex;
    justify-content: space-between;
    padding: 10px;
    background: rgb(82, 82, 245);
    border-bottom: 2px solid blue;
}

#menu {
    display: flex;
    justify-content: space-around;
    list-style: none;
}

.menu-item {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100%;
    width: 75px;
}

.menu-item:hover {
    background: rgb(82,82,255);
}

.menu-item a {
    text-decoration: none!important;
    color: white;
}

</style>

___

Note: I've just used the same logo as in the icon in the tab above. You can do the same.

## Navbar HTML

Our navbar HTML will look exactly like this (Remove the test h1 tag and add this inside the body, I'll explain it thoroughly):

```html
    <section id="navbar-section">
        <nav>
            <img height="60px" id="logo" src="/logo.png" alt="myLogo">
            <ul id="menu">
                <li class="menu-item"><a href="/">Home</a></li>
                <li class="menu-item"><a href="#about-section">About us</a></li>
            </ul>
        </nav>
    </section>
```

### Explaining the elements

First we'll see the `<section></section>` tags. They're new right. But don't worry they act just like div's. No real effect and simply to contain some content. An HTML file can become very large, and seperating code and making it make sense is important.

You'll also see most of the elements have id's and classes and other special attributes. id's and classes are used so that we can select the element with css. If we wanted to select the `<img>` tag in css we could do:

```css
img {
    width: 300px;
}
```

But that will select ALL the images on the page. So we give it an id instead.
Classes act the same as id's except we add only to one element, and classes we add to many elements that we want to look the same.

## Special attributes

You'll also notice the `height, alt, src, href` attributes. Height directly sets the height of the image, otherwise it will display at it's natural size. Alt is just info about the img that displays if the image doesn't load. src is important, this is where the image is found. In your case, it's in the same directory/folder as your index.html. That's why we can just set it to `src="/logo.png"`.

You may also have noticed that the image tag has no closing tag. It's also one of those special self closing tags.

___

Currently the navbar looks like this as you might have seen if you've added the HTML:

___

<section width="100%">
        <nav>
            <img height="60px" id="logo" src="/logo.png" alt="myLogo">
            <ul >
                <li ><a href="#">Home</a></li>
                <li ><a href="#">About us</a></li>
            </ul>
        </nav>
</section>

___

> EEWWW!

## Styling the navbar

Let's slam all the styles on there and I'll go through them one by one. Add this to your css file (keeping the others).

```css
#navbar-section {
    width: 100%;
    overflow: hidden;
}

#navbar-section nav {
    display: flex;
    justify-content: space-between;
    padding: 10px;
    background: rgb(82, 82, 245);
    border-bottom: 2px solid blue;
}

#menu {
    display: flex;
    justify-content: space-around;
    list-style: none;
}

.menu-item {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100%;
    width: 100px;
}

.menu-item:hover {
    background: rgb(82,82,255);
}

.menu-item a {
    text-decoration: none;
    color: white;
}
```
Your navbar should now look like this:
<br>

___

<section id="navbar-section">
        <nav>
            <img height="60px" id="logo" src="/website-tut-1/logo.png" alt="myLogo">
            <ul id="menu">
                <li class="menu-item"><a href="/">Home</a></li>
                <li class="menu-item"><a href="#about-section">About us</a></li>
            </ul>
        </nav>
</section>

____


#### If you're reading this... It's too early. That's it for Part one. Soak that info, then come back here in a few days and let's finish this site! I'll start by explaining all the styles and then we'll build this:

<br>
<br>

<section id="navbar-section">
        <nav>
            <img height="60px" id="logo" src="/website-tut-1/logo.png" alt="myLogo">
            <ul id="menu">
                <li class="menu-item"><a href="/">Home</a></li>
                <li class="menu-item"><a href="#about-section">About us</a></li>
            </ul>
        </nav>
    </section>

<section id="hero-section">
    <div id="textHolder">
        <h1>Welcome to ZenTrader Logistics</h1>
        <p>We clear, forward and take care of your shipments!</p>
        <div class="callButton">
            <a id="callText" target="_blank" href="tel:+264814444777">Call us!</a>
        </div>
    </div>
</section>

<style>

    #hero-section {
        display: flex;
        align-items: center;
        width: 100%;
        overflow: hidden;
        min-height: 100%;
        background-image: url('/website-tut-1/ZenTradersHero.jpg');
        background-size: cover;
        background-position: center;
    }

    #textHolder {
        display: flex;
        align-items: center;
        border-radius: 5px;
        flex-direction: column;
        background: rgba(0, 0, 0, 0.6);
        width: 35%;
        height: 50%;
        margin: 20px auto;
        padding: 20px;
        color: white;
        text-align: center;
    }

    /* call button */
    .callButton {
        background: rgb(80,80,240);
        width: 60px;
        padding: 15px 25px;
        border-radius: 2px;
        box-shadow: 1px 1px 1px rgba(255,255,255,0.3);
        transition: all 300ms;
    }

    .callButton a {
        color: white;
        text-decoration: none;
    }

    .callButton:hover {
        transform: scale(1.05);
        cursor: pointer;
    }
</style>

<br>
<br>

Did you enjoy it so far? Would you mind sharing [this link?](https://kaizenmedia.co.za/webdev/build-a-website-from-scratch.html) on your social media?