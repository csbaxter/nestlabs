# CSS

## Make Your Web Page Look Cool!

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

## Where do I start?

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

{% next %}

**Next**, let's fix the size of the image. The image I imported, `prudence.jpg` is much too big for this web page, and perhaps if you imported your own image, you would like to resize that as well. Again, sizes of elements can be determined by pixels, or percentage of the web page (or as we'll soon see a div that it's contained in). Let's make this image exactly 300 pixels wide. If we don't give it a width, it will automatically be sized to a height that's proportional.

To do this add a unique identifier or `id` to the `<img>` tag for your image. If you chose to use the term "prudence" as your `id`, your code would look like this:

```html
<img id="prudence" alt="Prudence" src="prudence.png">
```

Then we could add the new width of our image into the `<style>` section on top:

```css
<style>
  h1 {
    text-align: center;
  }
  #prudence {
    width: 300px;
  }
</style> 
```

Notice we use a hashtag, `#` in front of the `id`, "prudence". This is called a `CSS Selector`. We use a `#` in front of an `id` in `CSS` to tell our program that we are refering to the element with an `id` of "prudence.

{% next %}

To keep the text and image from being so close to the left margin of our web page, we can wrap this in a `div` or a section of our `HTML` document, with a width of 80% of whatever width our browser is open to. Let's give this `div` a `class` named "continer" and style it with `CSS`. A class also identifies code in between it's open and close `HTML` tags, however unlike an `id` it's not necessarily unique. We use a dot in front of the class name (as in `.container`) to refer to a class in `CSS`.

So our `HTML` might now look something like this:

```html
<div class="container">
  <p>Prudence is a rescue dog we adopted three years ago.</p>
  <img id="prudence" alt="Prudence" src="prudence.png">
  <p>We adopted her from <a href="https://www.bideawee.org/">Bidawee</a>.</p>
</div>       
```

We can describe the width of this `div` in `CSS` as 80%. We can also center the entire `div` in our browswer page by using `margin: auto`. 

Inside the `<style></style>` tags and after the close brace styling the "prudence" `id`, add:

```css
.container {
  width: 80%;
  margin: auto;
}
```
{% next %}

## Now add your own CSS!

Feel free to browse around the `CSS` pages in [W3 Schools](https://www.w3schools.com/css/) and continue to style your page with additional featuers such as different fonts, colors, and sizes of your elements. Feel free to experiment and have fun!


## To get more help with CSS

* [CSS](https://www.w3schools.com/css/)

## How to Submit

You may then submit by typing in at the command line:

submit50 cs50nestm/checks/2019/css


