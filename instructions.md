# Agenda: Build your first personal portfolio website!*
* Or whatever you want *

## What is HTML?
HTML is a type of markup language used to communicate content.

## What is CSS?
CSS is a type of markup language used to communicate styling.

## What are Classless CSS Frameworks?
Frameworks like MVP.css are prebuilt stylesheets with styling already written for the majority of commonly used tags in html. For instance, <img>, <a>, <p>.

# Getting Started!
1. Open these instructions
2. Open up replit and make a new HTMl,CSS,JS type repl.
3. Create an index.html file.

## index.html
Now that you have your home page file, you need to put stuff in it. Specifically content. A recommended way of starting is by using a boilerplate. Look below!
```
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Hello, world!</title>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <meta name="description" content="" />
  <link rel="stylesheet" type="text/css" href="style.css" />
</head>
<body>
  <header>
  </header>
  <main>
  </main>
</body>
</html>
```
This is what you want in your index.html

** Next Step **
You want to import the MVP.CSS framework. See where in the boilerplate is says `<link rel="stylesheet" type="text/css" href="style.css" />`.
We want to change that. It should say the link to our css framework. 
** https://unpkg.com/mvp.css@1.12/mvp.css **
Consequently that line of code should look like this: ` <link rel="stylesheet" href="https://unpkg.com/mvp.css@1.12/mvp.css">  `

Now you have imported a boilerplate and imported the CSS framework. Now its time to write HTML!

## Writing HTML
You have to write tags with content inside them. Where to begin? Start from top down. The top of the website has the navbar, the bottom the footer, and the middle being everything else.

### Navbar
A navbar is what you use to navigate to different pages. Almost every website has them these days. Fundamentally, its just a bar at the top of the screen with styled links.
```
<nav>
      <a href='/'>Home</a>
      <ul>
        <li><a href="/about.html">About</a></li>
        <li><a href="/example.html">Example</a></li>
      </ul>
    </nav>
```
The navbar is going to be put into the header section. That means between the `<header>` and `</header>`.
** HIT RUN TO TEST **

If successful you should see a navbar now. You can edit the words. If you want to change where the links go to, just make sure that is starts with a / and you make sure the change is reflected everywhere.
