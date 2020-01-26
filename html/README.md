# HTML

## Getting Ready

Beyond introducing you to web programming, the overarching goal of this problem is to empower you to teach yourself new languages so that you can stand on your own at the end of the year. We’ll guide you through each, but if you nonetheless find yourself Googling and asking lots of questions of classmates and staff, rest assured you’re doing it right!

First consider joining Daven for a tour of `HTML`. Focus for now on the `HTML`. We'll add in `CSS` in the next lab.

{% video https://www.youtube.com/watch?v=dM5V1epAbSs %}

{% next %}

# What do I do now?

Note there is already an `HTML` file, `mypage.html` set up for you in the sandbox on the right. Your job is to add several `HTML` tags with a title, some text, a picture and a link.

To view the your website, type in

```
http-server
```

into the terminal window, and then click on the refresh button under the brower tab on the right. Then click on the `mypage.html` link and you can preview your page.

Once `http-server` is running, you can preview any changes just by clicking on the refresh button.

**First**, let's add a heading to the top of your page.
 
Right under the first `<body>` tag, add an open and close `<h1>` tag with your name as follows:

```html
<h1>Margaret Tanzosh</h1>
```

With your name instead of mine!

**Second**, add a picture of yourself, or something you like using `<img>` tags.

If you find a picture of yourself online, or email one to yourself, you can drag the '.jpg' or '.png' file into your workspace. Make sure the name of the file has no spaces in it. If I had a picture saved as a `mtanzosh.png` in my workspace (click on the directory sidebar foler icon to the left of the `mypage.html` tab to see the files in your workspace), I could then import it as

```html
<img alt="Tanzosh" src="mtanzosh.png">
```                                    

**Third**, add a paragraph about yourself, under the `<img>` tag using paragraph tabs:

```html
<p>This is information about me!</p>
```

**Fourth**, add a link to your favorite website, using an anchor tag:

```html
<a href="https://www.google.com">A website I use all the time!</a>
```

Because this assignment will result in something different for each person, there’s no check50 for this one. Make sure that you’ve included everything listed above and you have no broken links or permission issues and you should be good to go.

## How to View Your Web Page

Type http-server in the terminal and then refresh the browser tab!

## To get more help with HTML and CSS

* [HTML](https://www.w3schools.com/html/)

* [CSS](https://www.w3schools.com/css/)

## How to Submit

You may then submit by typing in at the command line:

submit50 cs50/2018/ap/unit5


