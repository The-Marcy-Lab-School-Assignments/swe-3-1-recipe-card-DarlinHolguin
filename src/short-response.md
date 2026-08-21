# Short Response Questions

Answer the following questions in your own words. Each response should be 2-4 sentences.

## Question 1: HTML Structure

What is the difference between the `<head>` and `<body>` sections of an HTML document? What kind of content goes in each?

**Your Answer:**
The difference between the `<head>` & `<body>` is that on the actual website, we are able to see content put within the `<body>`. The `<head>` section contains metadata, the page title, and links to any CSS or JS(if your application has Javascript file) files that the browser needs, but the user never sees this information.

## Question 2: Semantic HTML

Why should we use semantic elements like `<header>`, `<main>`, and `<footer>` instead of using `<div>` tags for everything?

**Your Answer:**
We should use semantic elements like `<header>` `<main>`, and `<footer>` instead of `<div>` because it illustrates a clearer purpose to other developer/s who are also working on the application as well as giving meaning to browsers and screen readers. `<div>` is also a non-semantic element.

## Question 3: CSS Selectors

Given the following HTML:

```html
<ul>
  <li class="vegetable">Carrots</li>
  <li class="vegetable">Broccoli</li>
  <li class="fruit" id="favorite">Mango</li>
</ul>
```

Write THREE different CSS rules:

1. One that makes ALL list items have a `yellow` background
2. One that makes only the vegetables have `green` text color
3. One that makes only the Mango `bold`

**Your Answer:**

```css
ul > li {
  background-color: yellow;
}

.vegetable {
  color: green;
}

#favorite {
  font-weight: bold;
}
```

## Question 4: The Box Model

In your own words, explain the four parts of the CSS box model (content, padding, border, margin). What is the purpose of each part?

**Your Answer:**
The four parts of the CSS box model

- **Content** - The main part of the HTML element that we see, things like images and text are shown here.

- **Padding** - The padding is the spacing that is in between the content and the border. It can also act as background color.

- **Border** - The border is the line around the padding. It contains 3 values which are width, style, and color.

- **Margin** - Creates space outside of the border, it separates an element from other elements.

## Question 5: Box-Sizing

What problem does `box-sizing: border-box` solve? Why do we include it in a CSS reset at the top of our CSS files?

**Your Answer:**
The problem that `box-sizing: border-box` solves is that by default, when you set a `width` on an element, the **padding** and the **border** gets added on top of that. Meaning that it would be making the element wider than you actually wanted it to be. With `box-sizing: border-box`, the width you set **includes** the content, as well as both padding and border around it all together, so the element itself stays exactly to the size that you set it to.

The reason as to why we include it in a CSS RESET at the top of our CSS files is so that this basically becomes the automatic default layout across the whole application or project, basically setting a rule in our file to always follow and apply that behavior across every element on the page.

## Question 6: Display Property

What is the difference between `display: block`, `display: inline`, and `display: inline-block`? Give an example of when you might use `inline-block`.

**Your Answer:**
The difference between block and inline is that `display: block` takes up the full width available while also allowing you to set their width and height. Inline elements `display: inline` sit next to each other on the same line, however unlike block elements you cannot set the width and height, only on the horizontal axis. When using `display: inline-block` it's a combination of both block and inline elements. They align next to each other similar to inline but you are able to still set the width and height similar to block.

An example of when I'd use inline-block is a button and inside there's an arrow icon next to "download" text. Here I would want to use inline-block so that I can have the icon and text aligned the right way while keeping the button at a fixed height and width.
