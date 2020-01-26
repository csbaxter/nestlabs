# CSS

## Make your page look cool!

To style webpages, we’ll use another language, CSS, Cascading Style Sheets. CSS describes how HTML elements are to be displayed on screen, paper, or in other media and is a very important part of web design.

Consider joining Joseph for a tour of CSS:

{% video https://www.youtube.com/watch?v=kg0ZOmUREwc %}  

{% next %}

## What You Can Do with CSS

There are lot more things you can do with CSS.

* You can easily apply same style rules on multiple elements.
* You can control the presentation of multiple pages of a website with a single style sheet.
* You can present the same page differently on different devices.
* You can style dynamic states of elements such as hover, focus, etc. that isn't possible otherwise.
* You can change the position of an element on a web page without changing the markup.
* You can alter the display of existing HTML elements.
* You can transform elements like scale, rotate, skew, etc. in 2D or 3D space.
* You can create animations and transitions effects without using any JavaScript.

*- from tutorialrepublic.com*

{% next %}

# Where do I start?

Start by previewing the distribution code on the right. Remember to preview a web page, type in:

```
http-server
```

into the terminal window, and then click on the refresh button under the brower tab on the right. Then click on the `mypage.html` link and you can preview your page.

The page has a picture of my dog, Prudence, but it's not styled very well. Now that you know `HTML` feel free to edit the text, and add your own picture instead.

Let's start by centering the heading. There are many ways of doing this with `CSS`. You can add style attributes directly into your `HTML` tags, use a `<style>` element in the `<head>` section, or link an external `CSS` file that you link into the `<head>` section of your `HTML`. 

We'll add our `CSS` to the top of the `HTML` file on the right in between the `<style></style>` tags. If we want to center all `h1` heading tags, we can use this tag directly in our CSS as follows:

```css
<style>
  h1 {
    text-align: center;
  }
</style> 
```

Add this code into your `HTML` on the right and see what happens.

**Second**, add a picture of yourself, or something you like using `<img>` tags.

If you find a picture of yourself online, or email one to yourself, you can drag the '.jpg' or '.png' file into your workspace. Make sure the name of the file has no spaces in it. If I had a picture saved as a `mtanzosh.png` in my workspace (click on the directory sidebar foler icon to the left of the `mypage.html` tab to see the files in your workspace), I could then import it as

```html
<img alt="Tanzosh" src="mtanzosh.png">
```                                    

**Third**, add a paragraph about yourself, under the `<img>` tag using paragraph tags:

```html
<p>This is information about me!</p>
```

**Fourth**, add a link to your favorite website, using an anchor tag:

```html
<a href="https://www.google.com">A website I use all the time!</a>
```

And change the text in between the `<title></title>` tags and notice what happens to your Chrome (or other browser) tab on the top of your page!

Once you understand the structure of an `HTML` page, you can look up the many kinds of `HTML` tags to add other elements to your page as well. Feel free to experiment in this lab. Use the [W3 Schools reference](https://www.w3schools.com/html/) to get ideas on other elements for your page.

Do notice how tags inside of tags are indented. As when working in C, proper indentation makes your page much easier to read.

Because this assignment will result in something different for each person, there’s no check50 for this one. There is also no style50 for HTML, so check the indendentation yourself. Make sure that you’ve included everything listed above and you have no broken links and you should be good to go.

## How to View Your Web Page

Type http-server in the terminal and then refresh the browser tab!

## To get more help with HTML

* [HTML](https://www.w3schools.com/html/)

## How to Submit

You may then submit by typing in at the command line:

submit50 cs50nestm/checks/2019/html


