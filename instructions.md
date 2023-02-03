# Agenda: Build your first personal portfolio website!*
* Or whatever you want *



## What is HTML?
HTML is a type of markup language used to communicate content.



## What is CSS?
CSS is a type of markup language used to communicate styling.



## What are Classless CSS Frameworks?
Frameworks like MVP.css are prebuilt stylesheets with styling already written for the majority of commonly used tags in html. For instance, `<img>, <a>, <p>`.


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



**Next Step**
You want to import the MVP.CSS framework. See where in the boilerplate is says `<link rel="stylesheet" type="text/css" href="style.css" />`.
We want to change that. It should say the link to our css framework. 
**https://unpkg.com/mvp.css@1.12/mvp.css**
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



### Main
Between the `<main>` tags is where you are going to put the majority of the content for the page. The images, the paragraphs, the focus of whatever is supposed to be the page. 



**IMAGES**
`<figure>
        <img src="nameOfFile&extension">
      </figure>`
Figure is a tag that is styled by the classless css framework for images. So you need to have an img tag nested in a figure tag if you want the desired effects.

**Paragraphs**
Simple and useful, the `<p>` tag. Just wrap whatever you want to say within the p tag like such:
`<p>Hello World!</p>`


### What Now?
We have gone over making a boilerplate and navigating certain aspects of writing plain old html in a way our classless css framework understands how to style. You can put images, paragraphs, and a navbar. That should enable you to make a basic home page for your personal portfolio site. 

**NEXT STEPS(Challenges)**
1. Add new pages to your site. You will need to make a new file on replit and name it. Then reference the name in the links you added to your navbar so that the navbar will direct the users to the new pages.
2. Learn the other tags that the framework supports. Reference the MVP.CSS [Guide](https://andybrewer.github.io/mvp/#docs) and [w3schools](https://www.w3schools.com/tags/default.asp) reference guide. Add stuff like cards, tables, etc.
3. Also, check out [ehc.wiki](https://ehc.wiki) for the personal website worskhop resources. We have meaningful stuff on there. You can also contribute!

### Demo Code
```
<!DOCTYPE html>
<html lang="en">

<head>
  <title>Demo Site</title>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <meta name="description" content="" />
  <link rel="stylesheet" href="https://unpkg.com/mvp.css@1.12/mvp.css">
</head>

<body>
  <header>
    <nav>
      <a href='/'>Home</a>
      <ul>
        <li><a href="/about.html">About</a></li>
        <li><a href="/example.html">Example</a></li>
      </ul>
    </nav>
    <h1>CATS!</h1>
  </header>
  <main>
    <section>
      <figure> <img src="https://placekitten.com/200/287"> </figure>
    </section>
    <section>
      <p>Welcome to the Cat Photo Site!</p>
    </section>

  </main>
</body>

</html>
```

### Example Code(Kyle)
Does not include all types of tags!
```
<!DOCTYPE html>
<html lang="en">

<head>
  <title>Gateway Rug to Web Development 😨</title>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <meta name="description" content="" />
  <link rel="stylesheet" href="https://unpkg.com/mvp.css@1.12/mvp.css">
</head>

<body>
  <header>
    <nav>
      <a href='/'>HOME</a>
      <ul>
        <li><a href="/about.html">About</a></li>
        <li><a href="/example.html">Example</a></li>
      </ul>
    </nav>
    <h1>Kyle Liao: Programmer, Cybersecurity Student, @NYC🗽</h1>
    <p>Building Projects for Edison Hack Club, studying for Security+, attending hackathons, and almost at one year on
      duolingo!🦉</p>
  </header>
  <main>
    <section>
      <figure>
        <img src="https://kyleliao.tech/images/kyle.jpg">
      </figure>
    </section>
    <section>
      <aside>
        <h3>8+ Hackathons as of 2/2/2023</h4>
          <p>Code Overflow 2022, HackPHS 2022, HackTrin 2023</p>
      </aside>
      <aside>
        <h3>Programming Projects</h4>
          <p>Web Development: Front-end & Back-end</p>
          <p>Python: Flask, Discord Bots, etc</p>
          <p>More to come!</p>
      </aside>
      <aside>
        <h3>Edison Hack Club</h4>
          <p>Thanks for being here! 🤗</p>
      </aside>
    </section>
    <footer>
      <p>Contact Me</p>
      <p><a href="mailto:kyle@edisonhack.club">kyle@edisonhack.club</a></p>
    </footer>

  </main>
</body>

</html>
```

### Example Code(MVPCSS)
Includes all types of tags
```
<!DOCTYPE html>
<html lang="en">

<head>
    <link rel="icon" href="https://via.placeholder.com/70x70">
    <link rel="stylesheet" href="./mvp.css">

    <meta charset="utf-8">
    <meta name="description" content="My description">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>My title</title>
</head>

<body>
    <header>
        <nav>
            <a href="/"><img alt="Logo" src="https://via.placeholder.com/200x70?text=Logo" height="70"></a>
            <ul>
                <li>Menu Item 1</li>
                <li><a href="#">Menu Item 2</a></li>
                <li><a href="#">Dropdown Menu Item</a>
                    <ul>
                        <li><a href="#">Sublink with a long name</a></li>
                        <li><a href="#">Short sublink</a></li>
                    </ul>
                </li>
            </ul>
        </nav>
        <h1>Page Heading with <i>Italics</i> and <u>Underline</u></h1>
        <p>Page Subheading with <mark>highlighting</mark></p>
        <br>
        <p><a href="#"><i>Italic Link Button</i></a><a href="#"><b>Bold Link Button &rarr;</b></a></p>
    </header>
    <main>
        <hr>
        <section>
            <header>
                <h2>Section Heading</h2>
                <p>Section Subheading</p>
            </header>
            <aside>
                <h3>Card heading</h3>
                <p>Card content*</p>
                <p><small>*with small content</small></p>
            </aside>
            <aside>
                <h3>Card heading</h3>
                <p>Card content <sup>with notification</sup></p>
            </aside>
            <aside>
                <h3>Card heading</h3>
                <p>Card content</p>
            </aside>
        </section>
        <hr>
        <section>
            <blockquote>
                "Quote"
                <footer><i>- Attribution</i></footer>
            </blockquote>
        </section>
        <hr>
        <section>
            <table>
                <thead>
                    <tr>
                        <th></th>
                        <th>Col A</th>
                        <th>Col B</th>
                        <th>Col C</th>
                    </tr>
                </thead>
                <tr>
                    <td>Row 1</td>
                    <td>Cell A1</td>
                    <td>Cell B1</td>
                    <td>Cell C1</td>
                </tr>
                <tr>
                    <td>Row 2</td>
                    <td>Cell A2</td>
                    <td>Cell B2</td>
                    <td>Cell C2</td>
                </tr>
            </table>
        </section>
        <hr>
        <article>
            <h2>Left-aligned header</h2>
            <p>Left-aligned paragraph</p>
            <aside>
                <p>Article callout</p>
            </aside>
            <ul>
                <li>List item 1</li>
                <li>List item 2</li>
            </ul>
            <figure>
                <img alt="Stock photo" src="https://via.placeholder.com/1080x500?text=Amazing+stock+photo">
                <figcaption><i>Image caption</i></figcaption>
            </figure>
        </article>
        <hr>
        <div>
            <details>
                <summary>Expandable title</summary>
                <p>Revealed content</p>
            </details>
            <details>
                <summary>Another expandable title</summary>
                <p>More revealed content</p>
            </details>
            <br>
            <p>Inline <code>code</code> snippets</p>
            <pre>
                <code>
// preformatted code block
                </code>
            </pre>
        </div>
        <hr>
        <section>
            <form>
                <header>
                    <h2>Form title</h2>
                </header>
                <label for="input1">Input label:</label>
                <input type="text" id="input1" name="input1" size="20" placeholder="Input1">
                <label for="select1">Select label:</label>
                <select id="select1">
                    <option value="option1">option1</option>
                    <option value="option2">option2</option>
                </select>
                <label for="textarea1">Textarea label:</label>
                <textarea cols="40" rows="5" id="textarea1"></textarea>
                <button type="submit">Submit</button>
            </form>
        </section>
    </main>
    <footer>
        <hr>
        <p>
            <small>Contact info</small>
        </p>
    </footer>
</body>

</html>
```



