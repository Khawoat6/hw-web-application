# **Chapter 1 : Introduction to HTML and CSS**

## **HyperText Markup Language (HTML)**

- ### Syntax

  ![Getting Started](chapter1-intro-to-html-and-css/images/img1.png)

  ```html
  <!-- HTML -->
  <h1>HTML</h1>
  <p>
    HyperText Markup Language (HTML) is a markup language used to describe the
    structure of a web page.
  </p>
  <p>
    We can use it to differentiate such content as:
  </p>
  <ul>
    <li>headings</li>
    <li>lists</li>
    <li>links</li>
    <li>images</li>
  </ul>
  <p>
    Want to
    <a href="https://www.packtpub.com/web-development"
      >learn more about web development?</a
    >
  </p>
  ```

- ### Content Types

  ```
  Metadata
  Flow
  Sectioning
  Phrasing
  Heading
  Embedded
  Interactive
  ```

- ### The HTML Document

  ```html
  <html>
    <head>
      <title>HTML Document structure</title>
    </head>
    <body>
      <div>
        <h1>Heading</h1>
        <p>First paragraph of text.</p>
        <p>Second paragraph of text.</p>
      </div>
    </body>
  </html>
  ```

- ### The HTML DOM

  ```js
  <script>
    const anchorElement = document.createElement('a'); anchorElement.href = '#';
    anchorElement.textContent = 'Click me!'; const p =
    document.querySelector('.parent'); p.appendChild(anchorElement);
  </script>
  ```

- ### The Doctype Declaration
  ```html
  <!DOCTYPE html>
  ```

## **Structuring an HTML Document**

- ### HTML
  ```html
  <!DOCTYPE html>
  <html lang="en"></html>
  ```
- ### Head

  ```html
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <title>Page Title</title>
    </head>
  </html>
  ```

- ### Body

  ```html
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <title>Page Title</title>
    </head>
    <body></body>
  </html>
  ```

- ### Our First Web Page
- ### _Exercise 1.01: Creating a Web Page_

  ![Getting Started](chapter1-intro-to-html-and-css/images/ex1-01.png)

- ### Metadata

  ```html
  <base href="http://www.example.com" />
  <link rel="stylesheet" href="/style.css" />

  <meta charset="utf-8" />

  <meta name="viewport" content="width=device-width, initial-scale=1" />
  ```

- ### _Exercise 1.02: Adding Metadata_

  ![Getting Started](chapter1-intro-to-html-and-css/images/ex1-02.png)

## **Mistakes in HTML**

```html
<p>
Learn about <a href="https://www.packtpub.com/web-development">web development</a>. Try out some of the <a href="https://www.packtpub.com/free-learning">Free learning on the Packt site.
</p> <p>
Lorem ipsum... </p>
```

```html
<body>
  <main id="main1"><!-- main content here ... --></main>
  <main id="main2"><!-- more main content here ... --></main>
</body>
```

```html
<body>
  <main id="main1"><!-- main content here ... --></main>
  <main id="main2" hidden><!-- more main content here ... --></main>
</body>
```

## **Validating HTML**

```link
https://validator.w3.org/
```

- _Exercise 1.03: Validation_
- _Exercise 1.04: Validation Errors_
- _Activity 1.01: Video Store Page Template_

### CSS

- Syntax
  ```css
  p {
    color: red;
    font-weight: bold;
    text-decoration: underline;
  }
  ```
- CSS Rule Set

  ![Getting Started](chapter1-intro-to-html-and-css/images/img2.png)

- Adding Styles to a Web Page
- _Exercise 1.05: Adding Styles_

  ![Getting Started](chapter1-intro-to-html-and-css/images/ex1-05.png)

- _Exercise 1.06: Styles in an External Fils_

### CSSOM

### CSS Selectors

```css
h1::first-letter {
  font-size: 5rem;
}
p {
  color: white;
  background-color: black;
}
p:nth-of-type(odd) {
  color: black;
  background-color: white;
}
```

- Element, #ID and .Class

  ```css
  .class {
  }
  #id {
  }
  div {
  }
  ```

- The Universal Selectors (\*)

  ```css
  * {
  }
  ```

- Attribute Selectors

  ```css
  [attribute]
  [href]
  [attribute=value]
  [attribute^=value]
  [attribute$=value]
  [attribute*=valule]
  ```

- Pseudo-classes (:)

  ```css
  :link
  :hover
  :visited
  :active
  :first-child
  :last-child
  :nth-child()
  :nth-last-child()
  :first-of-type
  :last-of-type
  :nth-of-type()
  :nth-last-of-type()
  ```

  ```css
  a:link,
  a:visited {
    color: deepskyblue;
    text-decoration: none;
  }
  a:hover,
  a:active {
    color: hotpink;
    text-decoration: dashed underline;
  }
  ```

- Pseudo-elements (::)

  ```css
  ::before
  ::after
  ::first-letter
  ::first-line
  ::selection
  ::backdrop
  ```

- Combining Selectors

  ```css
  .primary li.primary;
  ```

- _Exercise 1.07: Selecting Elements_

  ![Getting Started](chapter1-intro-to-html-and-css/images/ex1-07.png)

### CSS Specificity

### The Special Case of `!important`

```css
/* CSS */
div.media {
  display: block;
  width: 100%;
  float: left;
}
.hide {
  display: none;
}
```

```html
<!-- HTML -->
<div class="media hide">
  ...Some content
</div>
```

```css
.hide {
  display: none !important;
}
```

- _Activity 1.02: Styling the Video Store Template Page_

### Dev Tools

- The Top Bar

  ```
  Console
  Elements ***
  Sources
  Network
  Performance
  ```

- The Element Tap

# Chapter 2: Structure and Layout

## Introduction

## Structural Elements

```html
<header></header>
<nav></nav>
<article></article>
<section></section>
<aside></aside>
<footer></footer>
```

### The header Tag

```html
<header>
  ... heading, logo, nav goes here
  <header></header>
</header>
```

### The footer Tag

```html
<footer>
  ... copyright, list of links go here
  <footer></footer>
</footer>
```

### The section Tag

```html
<section>
  ... main content
</section>
```

### The article Tag

```html
<article>
  <section>
    ...primary blog content
  </section>
  <section>
    ...secondary blog content
  </section>
</article>
```

### The nav Tag

```html
<navigation> ... list of links go here </navigation>
```

### The aside Tag

```html
<aside>
  ... indirectly related content goes here
</aside>
```

### The div Tag

```html
<div class="sidebar">
  ... indirectly related content goes here
</div>
<div class="navigation">
  <div class="navigation-inner">... navigation links go here</div>
</div>
```

### A News Article Web Page

```a
https://theguardian.com
https://bbc.co.uk/news
```

### _Exercise 2.01: Marking up the Page_

![Getting Started](chapter2-structure-and-layout/images/ex2-01.png)

### Wireframes

### _Activity 2.01: Video Store Home Page_

![Getting Started](chapter2-structure-and-layout/images/activity2-01.png)

---

## CSS Page Layouts

```css
float
flex
grid
```

### Video Store Product Page

### Float-Based Layout

- The float Property

  ```css
  float: right;
  float: left;
  float: none;
  ```

- the width Property

  ```css
  width: 100px;
  width: 25%;
  ```

- Claring Floated Element

  ```css
  /* CSS */
  section {
    overflow: hidden;
  }
  div {
    float: left;
    width: 25%;
  }
  ```

  ```html
  <!-- HTML -->
  <section>
    <div>product 1</div>
    <div>product 2</div>
    <div>product 3</div>
    <div>product 4</div>
    <div>product 5</div>
    <div>product 6</div>
    <div>product 7</div>
    <div>product 8</div>
  </section>
  ```

### Flex-Based Layout

- The flex Container

  ```css
  display: flex;
  ```

  ```css
  flex-wrap: wrap;
  ```

- The flex Items
  `css flex-basis: 25%;`

  ```html
  <!-- HTML -->
  <section>
    <div>product 1</div>
    <div>product 2</div>
    <div>product 3</div>
    <div>product 4</div>
    <div>product 5</div>
    <div>product 6</div>
    <div>product 7</div>
    <div>product 8</div>
  </section>
  ```

  ```css
  /* CSS */
  section {
    display: flex;
    flex-wrap: wrap;
  }
  div {
    flex-basis: 25%;
  }
  ```

### Grid-Based Layout

- The grid Container

  ```css
  display: grid;
  ```

  ```css
  grid-template-columns: auto auto;
  ```

- The grid Items

### _Exercise 2.02: A grid-Based Layout_

![Getting Started](chapter2-structure-and-layout/images/ex2-02.png)

## The Box Model

```css
margin
border
padding
content
width
height
```

### Content Box

```css
width: 200px;
height: 100px;
```

### The padding Property

```css
padding: 50px;
padding: 50px 0;
padding-top: 10px;
padding-right: 10px;
padding-bottom: 10px;
padding-left: 10px;
```

```css
width: 200px;
height: 100px;
padding: 25px;
```

### The border Property

```css
border: 5px solid red;
border-top: 5px solid red;
border-right: 15px dotted green;
border-bottom: 10px dashed blue;
borber-left: 10px double pink;
```

```css
width: 200px;
height: 100px;
padding: 25px;
border: 10px solid black;
```

### The margin Property

```css
margin: 50px;
margin: 50px 0;
margin-top: 10px;
margin-right: 10px;
margin-bottom: 10px;
margin-left: 10px;
```

```css
width: 200px;
height: 100px;
padding: 25px;
border: 10px solid black;
margin: 25px;
```

### _Exercise 2.03: Experimenting with the Box Model_

![Getting Started](chapter2-structure-and-layout/images/ex2-03.png)

### Putting It All Together

### _Exercise 2.04: Home Page Revisited_

![Getting Started](chapter2-structure-and-layout/images/ex2-04.png)

### _Exercise 2.05: Video Store Product Page Revisited_

![Getting Started](chapter2-structure-and-layout/images/ex2-05.png)

### _Activity 2.02: Online Clothes Store Home Page_

![Getting Started](chapter2-structure-and-layout/images/activity2-02.png)

# Chapter 3: Text and Typography

## Table of Contents

[Text-Based Elements](#text-based-element)

- [Headings](#Headings)
- [Paragraphs](#paragraphs)
- [Inline Text Elements](#inline-text-elements)
- [Lists](#lists)
- [Exercise 3.01: Combining Text-Based Elements](#Exercise-3.01:-Combining-Text-Based-Elements)

[Semantic Markup](#Semantic-Markup)

[Styling Text-Based Elements](#Styling-Text-Based-Elements)

- [CSS Resets](#CSS-Resets)
- [CSS Text Properties](#CSS-Text-Properties)
- [CSS Font Properties](#CSS-Font-Properties)
- [The display Properties](#The-display-Properties)
- [Video Store Product Page (Revisied)](<#Video-Store-Product-Page-(Revisied)>)
- [Exercise 3.02: Navigation](#Exercise-3.02:-Navigation)

[Breadcrumbs](#Breadcrumbs)

- [Exercise 3.03: Breadcrumb](#Exercise-3.03:-Breadcrumb)
- [Exercise 3.04: Page Heading and Introduction](#Exercise-3.04:-Page-Heading-and-Introduction)
- [Exercise 3.06: Putting It All Together](#Exercise-3.06:-Putting-It-All-Together)

## Text-Based Elements

```
- Headings
- Paragraphs
- Inline elements
- Lists
```

- ### Headings

  ```html
  <h1>Heading level 1</h1>
  <h2>Heading level 2</h2>
  <h3>Heading level 3</h3>
  <h4>Heading level 4</h4>
  <h5>Heading level 5</h5>
  <h6>Heading level 6</h6>
  ```

- ### Paragraphs

  ```html
  <p>
    Sit down awhile, And let us once again assail your ears, That are so
    fortified against our story,
  </p>
  ```

- ### Inline Text Elements

  ```html
  <p>I need to wake up <em>now</em>!</p>
  ```

  ```html
  <p>
    Before leaving the house <strong>remember to lock the front door</strong>!
  </p>
  ```

- ### Lists

  ```html
  <!-- Shopping list -->
  <ul>
    <li>Ice Cream</li>
    <li>Cookies</li>
    <li>Salad</li>
    <li>Soap</li>
  </ul>
  ```

  ```html
  <!-- Cheese on toast recipe -->
  <ol>
    <li>Place bread under grill until golden brown</li>
    <li>Flip the bread and place cheese slices</li>
    <li>Cook until cheese is golden brown</li>
    <li>Serve immediately</li>
  </ol>
  ```

  ```html
  <!-- Dictionary -->
  <dl>
    <dt>HTML</dt>
    <dd>Hypertext markup language</dd>
    <dt>CSS</dt>
    <dd>Cascading style sheets</dd>
  </dl>
  ```

- ### _Exercise 3.01: Combining Text-Based Elements_

  ![Getting Started](chapter3-text-and-typography/images/ex3-01.png)

## Semantic Markup

```html
<!-- Semantic markup -->
<h1>I am a top level page heading</h1>
<p>
  This is a paragraph which contains a word with
  <strong>strong</strong> significance
</p>
<!-- Non semantic markup -->
<div>I am a top level page heading</div>
<div>
  This is a paragraph which contains a word with
  <span>strong</span> significance
</div>
```

## Styling Text-Based Elements

- ### CSS Resets

  ```css
  * {
    margin: 0;
    padding: 0;
  }
  ```

  ```css
  /* http://meyerweb.com/eric/tools/css/reset/ v2.0 | 20110126
  License: none (public domain)
  */
  html,
  body,
  div,
  span,
  applet,
  object,
  iframe,
  h1,
  h2,
  h3,
  h4,
  h5,
  h6,
  p,
  blockquote,
  pre,
  a,
  abbr,
  acronym,
  address,
  big,
  cite,
  code,
  del,
  dfn,
  em,
  img,
  ins,
  kbd,
  q,
  s,
  samp,
  small,
  strike,
  strong,
  sub,
  sup,
  tt,
  var,
  b,
  u,
  i,
  center,
  dl,
  dt,
  dd,
  ol,
  ul,
  li,
  fieldset,
  form,
  label,
  legend,
  table,
  caption,
  tbody,
  tfoot,
  thead,
  tr,
  th,
  td,
  article,
  aside,
  canvas,
  details,
  embed,
  figure,
  figcaption,
  footer,
  header,
  hgroup,
  menu,
  nav,
  output,
  ruby,
  section,
  summary,
  time,
  mark,
  audio,
  video {
    margin: 0;
    padding: 0;
    border: 0;
    font-size: 100%;
    font: inherit;
    vertical-align: baseline;
  }
  /* HTML5 display-role reset for older browsers */
  article,
  aside,
  details,
  figcaption,
  figure,
  footer,
  header,
  hgroup,
  menu,
  nav,
  section {
    display: block;
  }
  body {
    line-height: 1;
  }
  ol,
  ul {
    list-style: none;
  }
  blockquote,
  q {
    quotes: none;
  }
  blockquote:before,
  blockquote:after,
  q:before,
  q:after {
    content: "";
    content: none;
  }
  table {
    border-collapse: collapse;
    border-spacing: 0;
  }
  ```

- ### CSS Text Properties

  ```css
  h1 {
    color: green;
  }
  p {
    color: #00ff00;
  }
  span {
    color: rgb(0, 255, 0);
  }
  p {
    text-align: center;
  }
  /* ขีดเส้นใต้หนังสือ */
  .underline {
    text-decoration: underline;
  }
  /* เส้นทับตัวหนังสือ */
  .line-through {
    text-decoration: line-through;
  }
  /* ตัวใหญ่หมด */
  .uppercase {
    text-transform: uppercase;
  }
  /* ตัวเล็กหมด */
  .lowercase {
    text-transform: lowercase;
  }
  /* อักษรตัวแรกใหญ่ */
  .capitalize {
    text-transform: capitalize;
  }
  /* ความชิดของแต่ละบรรทัด น้อย */
  .small-line-height {
    line-height: 0.5;
  }
  /* ความชิดของแต่ละบรรทัด มาก */
  .large-line-height {
    line-height: 1.5;
  }
  ```

- ### CSS Font Properties

  ```css
  body {
    font-family: "Times New Roman", Times, serif;
  }
  /* pixels */
  h1 {
    font-size: 50px;
  }
  p {
    font-size: 16px;
  }
  /* ems */
  h1 {
    font-size: 3.125em;
  }
  p {
    font-size: 1em;
  }
  span {
    font-weight: bold;
  }
  ```

- ### The display Properties

  ```css
  div {
    display: inline;
  }
  span {
    display: block;
  }
  ```

- ### Video Store Product Page (Revisied)

- ### _Exercise 3.02: Navigation_

  ![Getting Started](chapter3-text-and-typography/images/ex3-02.png)

## Breadcrumbs

- ### _Exercise 3.03: Breadcrumb_

  ![Getting Started](chapter3-text-and-typography/images/ex3-03.png)

- ### _Exercise 3.04: Page Heading and Introduction_

  ![Getting Started](chapter3-text-and-typography/images/ex3-04.png)

- ### _Exercise 3.05: Product Cards_

  ![Getting Started](chapter3-text-and-typography/images/ex3-05.png)

- ### _Exercise 3.06: Putting It All Together_

  ![Getting Started](chapter3-text-and-typography/images/ex3-06.png)

- ### _Activity 3.01: Converting a Newspaper Article to a Web Page_

# Chapter 4 : Forms

## Table Content

[Form Elements](#Form-Elements)

- [The form Element](#The-form-Element)
- [The input Element](#The-input-Element)
- [The label Element](#The-label-Element)
- [The textarea Element](#The-textarea-Element)
- [The fieldset Element](#The-fieldset-Element)
- [The select Element](#The-select-Element)
- [The button Element](#The-button-Element)
- [Exercise 4.01: Creating a Simple Form](#Exercise-4.01:-Creating-a-Simple-Form)

[Styling Form Elements](#Styling-Form-Elements)

- [Label, Textbox, and Textarea](#Label-Textbox-and-Textarea)
- [Buttons](#Buttons)
- [Select Boxes](#Select-Boxes)
- [Validation Styling](#Validation-Styling)
- [Exercise 4.02: Creating a Form with Validation Styling](#Exercise-4.02:-Creating-a-Form-with-Validation-Styling)
- [Video Store Forms](#Video-Store-Forms)
- [Exercise 4.03: New Account Signup Form](#Exercise-4.03:-New-Account-Signup-Form)
- [Exercise 4.04: Checkout Form](#Exercise-4.04:-Checkout-Form)
- [Activity 4.01: Building an Online Property Portal Website Form](#Activity-4.01:-Building-an-Online-Property-Portal-Website-Form)

[Summary](#Summary)

## Introduction

## Form Elements

- `form`
- `input`
- `label`
- `textarea`
- `fieldset`
- `select`
- `button`

* ### The form Element

  `form`, `action`, `method`, `get`, `post`

  ```html
  <form action="url_to_send_form_data" method="post">
    <!-- form elements go here -->
  </form>
  ```

- ### The input Element

  `type`, `name`, `value`, `maxlength`

  ```html
  <!-- text input -->
  <form action="url_to_send_form_data" method="post">
    <div>
      First name: <br />
      <input type="text" name="firstname" />
    </div>
    <div>
      Last name: <br />
      <input type="text" name="lastname" />
    </div>
  </form>
  ```

  ![Getting Started](chapter4-forms/images/img1.png)

  ```html
  <!-- maxlength -->
  <input type="text" name="username" maxlength="20" />
  ```

  ```html
  <!-- email input -->
  <form action="url_to_send_form_data" method="post">
    <div>
      Email: <br />
      <input type="email" name="email" />
    </div>
  </form>
  ```

  ![Getting Started](chapter4-forms/images/img2.png)

  ```html
  <!-- password input -->
  <form action="url_to_send_form_data" method="post">
    <div>
      Password: <br />
      <input type="password" name="password" />
    </div>
  </form>
  ```

  ![Getting Started](chapter4-forms/images/img3.png)

  ```html
  <!-- value -->
  <!-- checkboxes -->
  <form action="url_to_send_form_data" method="post">
    <div><input type="checkbox" name="color1" value="red" /> Red</div>
    <div><input type="checkbox" name="color2" value="green" /> Green</div>
    <div><input type="checkbox" name="color3" value="blue" /> Blue</div>
    ..
  </form>
  ```

  ![Getting Started](chapter4-forms/images/img4.png)

  ```html
  <!-- radio buttons -->
  <form action="url_to_send_form_data" method="post">
    <div><input type="radio" name="color" value="red" /> Red</div>
    <div><input type="radio" name="color" value="green" /> Green</div>
    <div><input type="radio" name="color" value="blue" /> Blue</div>
  </form>
  ```

  ![Getting Started](chapter4-forms/images/img5.png)

- ### The label Element

  `label`, `for`, `id`

  ```html
  <!-- text inputs with labels -->
  <form action="url_to_send_form_data" method="post">
    <div>
      <label for="first_name">First name:</label><br />
      <input type="text" name="firstname" id="first_name" />
    </div>
    <div>
      <label for="last_name">Last name:</label><br />
      <input type="text" name="lastname" id="last_name" />
    </div>
  </form>
  ```

  ![Getting Started](chapter4-forms/images/img6.png)

* ### The textarea Element

  `textarea`, `rows`, `cols`

  ```html
  <!-- textarea -->
  <form action="url_to_send_form_data" method="post">
    <div>
      <label for="first_name">First name:</label><br />
      <input type="text" name="firstname" id="first_name" />
    </div>
    <div>
      <label for="last_name">Last name:</label><br />
      <input type="text" name="lastname" id="last_name" />
    </div>
    <div>
      <label for="message">Message:</label><br />
      <textarea id="last_name" rows="5" cols="20"></textarea>
    </div>
  </form>
  ```

  ![Getting Started](chapter4-forms/images/img7.png)

- ### The fieldset Element

  `fieldset`

  ```html
  <!-- fieldset -->
  <form action="url_to_send_form_data" method="post">
    <fieldset>
      <div>
        <label for="first_name">First name:</label><br />
        <input type="text" name="firstname" id="first_name" />
      </div>
      <div>
        <label for="last_name">Last name:</label><br />
        <input type="text" name="lastname" id="last_name" />
      </div>
      <div>
        <label for="message">Message:</label><br />
        <textarea id="last_name" rows="5" cols="20"></textarea>
      </div>
    </fieldset>
    <p>Do you like HTML?</p>
    <fieldset>
      <div>
        <input type="radio" id="yes" />
        <label for="yes">Yes</label>
      </div>
      <div>
        <input type="radio" id="no" />
        <label for="no">No</label>
      </div>
    </fieldset>
  </form>
  ```

  ![Getting Started](chapter4-forms/images/img8.png)

* ### The select Element

  `select`, `option`

  ```html
  <!-- select -->
  <form action="url_to_send_form_data" method="post">
    <fieldset>
      <label for="countries">Country:</label><br />
      <select id="countries">
        <option value="england">England</option>
        <option value="scotland">Scotland</option>
        <option value="ireland">Ireland</option>
        <option value="wales">Wales</option>
      </select>
    </fieldset>
  </form>
  ```

  ![Getting Started](chapter4-forms/images/img9.png)

* ### The button Element

  `button`, `type`, `reset`, `submit`

  ```html
  <button type="submit">Submit</button>
  ```

* ### _Exercise 4.01: Creating a Simple Form_

  ![Getting Started](chapter4-forms/images/ex4-01.png)

## Styling Form Elements

- `Textbox`
- `Textarea`
- `Label`
- `Button`
- `Select box`
- `Validation styling`

* ### Label Textbox and Textarea

  `label`, `textarea`

  ```html
  <!-- HTML -->
  <form action="url_to_send_form_data" method="post">
    <div>
      <label for="first_name">First name:</label><br />
      <input
        type="text"
        name="firstname"
        id="first_name"
        placeholder="Your first name"
      />
    </div>
    <div>
      <label for="last_name">Last name:</label><br />
      <input
        type="text"
        name="lastname"
        id="last_name"
        placeholder="Your last name"
      />
    </div>
    <div>
      <label for="message">Message:</label><br />
      <textarea
        id="last_name"
        rows="5"
        cols="20"
        placeholder="Your message"
      ></textarea>
    </div>
  </form>
  ```

  ```css
  /* CSS */
  * {
    font-family: arial, sans-serif;
  }
  label {
    font-size: 20px;
  }
  div {
    margin-bottom: 30px;
  }
  input,
  textarea {
    border: 0;
    border-bottom: 1px solid gray;
    padding: 10px 0;
    width: 200px;
  }
  ```

  ![Getting Started](chapter4-forms/images/img10.png)

- ### Buttons

  `button`, `submit`

  ```html
  <!-- HTML -->
  <button type="submit">Submit</button>
  ```

  ```css
  /* CSS */
  button {
    background: #999;
    border: 0;
    color: white;
    font-size: 12px;
    height: 50px;
    width: 200px;
    text-transform: uppercase;
  }
  ```

  ![Getting Started](chapter4-forms/images/img11.png)

- ### Select Boxes

  `select`

  ```html
  <!-- HTML -->
  <div class="select-wrapper">
    <select id="countries">
      <option value="england">England</option>
      <option value="scotland">Scotland</option>
      <option value="ireland">Ireland</option>
      <option value="wales">Wales</option>
    </select>
  </div>
  ```

  ```css
  /* CSS */
  select {
    background: transparent;
    border: 0;
    border-radius: 0;
    border-bottom: 1px solid gray;
    box-shadow: none;
    color: #666;
    padding: 10px 0;
    width: 200px;
    -webkit-appearance: none;
  }
  .select-wrapper {
    position: relative;
    width: 200px;
  }
  .select-wrapper:after {
    content: "< >";
    color: #666;
    font-size: 14px;
    top: 8px;
    right: 0;
    transform: rotate(90deg);
    position: absolute;
    z-index: -1;
  }
  ```

  ![Getting Started](chapter4-forms/images/img12.png)

* ### Validation Styling

  `required`, `:valid`, `:valid`

- ### _Exercise 4.02: Creating a Form with Validation Styling_

  ![Getting Started](chapter4-forms/images/ex4-02.png)

* ### Video Store Forms
* ### _Exercise 4.03: New Account Signup Form_

  ![Getting Started](chapter4-forms/images/ex4-03.png)

* ### _Exercise 4.04: Checkout Form_

  ![Getting Started](chapter4-forms/images/ex4-04.png)

- ### _Activity 4.01: Building an Online Property Portal Website Form_

## Summary

# Chapter 5: Themes, Colors, and Polish

## Table Content

[Introduction](#Introduction)

- [The Markup](#The-Markup)
- [Inverting Colors](#Inverting-Colors)
- [New HTML Elements in the Theme](#New-HTML-Elements-in-the-Theme)
- [New CSS Background Properties](#New-CSS-Background-Properties)
- [Exercise 5.01: Creating a Dark Theme](#Exercise-5.01:-Creating-a-Dark-Theme)
- [Creating a Dark Theme with the HSL Function](#Creating-a-Dark-Theme-with-the-HSL-Function)
- [Exercise 5.02: Creating a Dark Theme Using hsl](#Exercise-5.02:-Creating-a-Dark-Theme-Using-hsl)
- [CSS Invert Filter](#CSS-Invert-Filter)
- [Exercise 5.03: Creating a Dark Theme with the CSS Invert Filter](#Exercise-5.03:-Creating-a-Dark-Theme-with-the-CSS-Invert-Filter)
- [CSS Hooks](#CSS-Hooks)
- [Exercise 5.04: Customizing a Theme with CSS Hooks](#Exercise-5.04:-Customizing-a-Theme-with-CSS-Hooks)
- [Activity 5.01: Creating Your Own Theme Using a New Color Palette](#Activity-5.01:-Creating-Your-Own-Theme-Using-a-New-Color-Palette)

[Summary](#Summary)

## Introduction

### The Markup

![Getting Started](chapter5-themes-colors-and-polish/images/img1.png)

### Inverting Colors

```link
https://www.colortools.net/color_complementary.html
```

### New HTML Elements in the Theme

- `pre` (preformatted element)
- `abbr` (abbreviation element)

### New CSS Background Properties

- `background-image`
- `background-repeat`
  - `repeat`
  - `space`
  - `round`
  - `no-repeat`

### _Exercise 5.01: Creating a Dark Theme_

![Getting Started](chapter5-themes-colors-and-polish/images/ex5-01.png)

### Creating a Dark Theme with the HSL Function

The HSL function allows you to update the color value of a property by using one of three arguments: **H**ue, **S**aturation, or **L**ightness:

- `H` represents the hue as an angle on the color wheel. You can specify this using degrees (or, programmatically, radians.) When provided as a unitless number, it is interpreted as degrees, with 0 as pure red, 120 as pure green, and 240 as pure blue.
- `S` represents the saturation, with 100% saturation being completely saturated, while 0% is completely unsaturated (gray). 50% is a "normal" color.
- `L` represents the saturation, with 100% saturation being completely saturated, while 0% is completely unsaturated (gray).

  ![Getting Started](chapter5-themes-colors-and-polish/images/img2.png)

### _Exercise 5.02: Creating a Dark Theme Using hsl_

![Getting Started](chapter5-themes-colors-and-polish/images/ex5-02.png)

### CSS Invert Filter

`filter: invert().`

![Getting Started](chapter5-themes-colors-and-polish/images/img3.png)

```html
<!DOCTYPE html>
<html lang="en-US">
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
    <title>Invert Filter</title>
    <style type="text/css">
      .invert {
        filter: invert(100%);
      }
    </style>
  </head>
  <body>
    <p>
      <img
        src="./assets/react-2019-7.jpg"
        width="100%"
        alt="a mural by the author"
      />
    </p>
    <p>
      <img
        src="./assets/react-2019-7.jpg"
        width="100%"
        alt="a mural by the author"
        class="invert"
      />
    </p>
  </body>
</html>
```

### _Exercise 5.03: Creating a Dark Theme with the CSS Invert Filter_

![Getting Started](chapter5-themes-colors-and-polish/images/ex5-03.png)

### CSS Hooks

```html
<!DOCTYPE html>
<html lang="en-US">
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
    <title>Using CSS hooks</title>
    <style type="text/css">
      .tag-css {
        background: #003366;
      }
      .tag-html {
        background: #006600;
      }
      .tag-javascript {
        background: #660000;
      }
    </style>
  </head>
  <body class="tag-css"></body>
</html>
```

### _Exercise 5.04: Customizing a Theme with CSS Hooks_

![Getting Started](chapter5-themes-colors-and-polish/images/ex5-04.png)

### _Activity 5.01: Creating Your Own Theme Using a New Color Palette_

## Summary

<!-- CONTACT -->

# **Chapter 6: Responsive Web Design and Media Queries**

## **Table Content**

[Mobile-First](#Mobile-First)

- [Responsive Web Design](#Responsive-Web-Design)
- [Responsive Viewport](#Responsive-Viewport)
- [Understanding Basic Media Queries](#Understanding-Basic-Media-Queries)
- [Exercise 6.01: Using Media Queries to Change the Page Layout](#Exercise-6.01:-Using-Media-Queries-to-Change-the-Page-Layout)
- [Device Orientation Media Queries](#Device-Orientation-Media-Queries)
- [Exercise 6.02: Using Media Queries to Detect Device Orientation](#Exercise-6.02:-Using-Media-Queries-to-Detect-Device-Orientation)
- [Combining Multiple Media Queries](#Combining-Multiple-Media-Queries)
- [Print Stylesheets](#Print-Stylesheets)
- [Exercise 6.03: Generating a Printable Version of a Web Page Using CSS Media Queries](#Exercise-6.03:-Generating-a-Printable-Version-of-a-Web-Page-Using-CSS-Media-Queries)
- [Activity 6.01: Refactoring the Video Store Product Cards into a Responsive Web Page](#Activity-6.01:-Refactoring-the-Video-Store-Product-Cards-into-a-Responsive-Web-Page)

## **Mobile-First**

### Responsive Web Design

### Responsive Viewport

- `width`
- `device-width`
- `initial-scale`
- `maximum-scale`

  ```html
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="UTF-8" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <title>Web Responsive</title>
    </head>
    <body>
      <h1>HTML and CSS</h1>
      <p>How to create a modern, responsive website with HTML and CSS</p>
    </body>
  </html>
  ```

### Understanding Basic Media Queries

- `@media`
- `@media only screen and (max-width: 768[x])`

  ![Getting Started](chapter6-responsive-web-design-and-media-queries/images/img1.png)

  ```css
  /* 0-768px is blue color */
  @media only screen and (max-width: 768px) {
    p {
      color: blue;
    }
  }
  ```

  ![Getting Started](chapter6-responsive-web-design-and-media-queries/images/img2.png)

  ```css
  /* 769 up is a red color */
  @media only screen and (min-width: 769px) {
    p {
      color: red;
    }
  }
  ```

  ![Getting Started](chapter6-responsive-web-design-and-media-queries/images/img3.png)

  ```css
  /* between 480-768 is a purple color */
  @media only screen and (min-width: 480px) and (max-width: 768px) {
    p {
      color: purple;
    }
  }
  ```

  ![Getting Started](chapter6-responsive-web-design-and-media-queries/images/img4.png)

  ```css
  /* height 500 up background-color is pink */
  @media only screen and (min-height: 500px) {
    body {
      background-color: pink;
    }
  }
  ```

  ![Getting Started](chapter6-responsive-web-design-and-media-queries/images/img5.png)

### _Exercise 6.01: Using Media Queries to Change the Page Layout_

![Getting Started](chapter6-responsive-web-design-and-media-queries/images/ex6-01.png)

### Device Orientation Media Queries

- `@media (orientation: landscape)`
- `@media (orientation: portrait)`

  ```html
  <!-- Example 6.01 -->
  <html>
    <head>
      <meta name="viewport" content="width=device-width, initial-scale=1" />
      <style type="text/css">
        p.warning {
          display: none;
          background: yellow;
          padding: 10px;
          font-size: 25px;
          margin: 0;
        }

        @media (orientation: landscape) {
          p.warning {
            display: block;
          }
        }
        img {
          width: 100%;
          height: auto;
        }
      </style>
    </head>
    <body>
      <p class="warning">
        Your device is in landscape orientation, this webpage is best viewed in
        portrait mode.
      </p>
      <img src="http://placehold.it/768x1024" alt="" />
    </body>
  </html>
  ```

  ```css
  @media (orientation: landscape) and (min-width: 400px) and (max-width: 768px);
  ```

  ![Getting Started](chapter6-responsive-web-design-and-media-queries/images/img6.png)

  > _Orientation warning demo on a tablet and mobile device_

  ```html
  <html>
    <head>
      <meta name="viewport" content="width=device-width, initial-scale=1" />
      <style type="text/css">
        p.warning {
          display: none;
          background: yellow;
          padding: 10px;
          font-size: 25px;
          margin: 0;
        }

        @media (orientation: landscape) and (min-width: 400px) and (max-width: 768px) {
          p.warning {
            display: block;
          }
        }
        img {
          width: 100%;
          height: auto;
        }
      </style>
    </head>
    <body>
      <p class="warning">
        Your device is in landscape orientation, this webpage is best viewed in
        portrait mode.
      </p>
      <img src="http://placehold.it/768x1024" alt="" />
    </body>
  </html>
  ```

### _Exercise 6.02: Using Media Queries to Detect Device Orientation_

![Getting Started](chapter6-responsive-web-design-and-media-queries/images/ex6-02.png)

### Combining Multiple Media Queries

```css
/*
    width: 0-319 is pink color
    width: 320-480 is red color
    width: 481-1279 is pink color
    width: 1280 up is red color
*/
@media screen and (max-width: 480) and (min-width: 320), (min-width: 1280px) {
  body {
    background: red;
  }
}
```

![Getting Started](chapter6-responsive-web-design-and-media-queries/images/img7.png)

### Print Stylesheets

- `<link />`
- `@media`

  ```css
  <link rel="stylesheet" media="print" href="print.css" />
  ```

### _Exercise 6.03: Generating a Printable Version of a Web Page Using CSS Media Queries_

![Getting Started](chapter6-responsive-web-design-and-media-queries/images/ex6-03.png)

### _Activity 6.01: Refactoring the Video Store Product Cards into a Responsive Web Page_

# **Chapter 7 : Media - Audio Video and Canvas**

[Introduction](#Introduction)
[Audio](#Audio)

- [Exercise 7.01: Adding Audio to a Web Page](#Exercise-7.01:-Adding-Audio-to-a-Web-Page)
- [Attributes](#Attributes)
  - [The Autoplay Attribute](#The-Autoplay-Attribute)
  - [The preload Attribute](#The-preload-Attribute)
  - [The loop Attribute](#The-loop-Attribute)
  - [The controls Attribute](#The-controls-Attribute)
- [Styling Audio Controls](#Styling-Audio-Controls)
- [Exercise 7.02: Styling Controls](#Exercise-7.02:-Styling-Controls)
- [Multiple Sources](#Multiple-Sources)

[The video Element](#The-video-Element)

- [Attributes](#Attributes)
  - [The width and height Attributes](#The-width-and-height-Attributes)
  - [The poster Attribute](#The-poster-Attribute)
- [Exercise 7.03: Adding Video to a Web Page](#Exercise-7.03:-Adding-Video-to-a-Web-Page)

[Limitations](#Limitations)

[The track Element](#The-track-Element)

- [Adding Subtitles](#Adding-Subtitles)
- [Exercise 7.04: Adding Subtitles](#Exercise-7.04:-Adding-Subtitles)

[Images](#Images)

- [The img Element](#The-img-Element)
- [The picture Element](#The-picture-Element)
- [Programmable Graphics](#Programmable-Graphics)
  - [The svg Element](#The-svg-Element)
  - [The canvas Element](#The-canvas-Element)
    - [Checking for canvas Support](#Checking-for-canvas-Support)
    - [Drawing in canvas](#Drawing-in-canvas)
    - [The canvas Grid](#The-canvas-Grid)
    - [Drawing a Rectangle](#Drawing-a-Rectangle)
    - [Drawing a Circle](#Drawing-a-Circle)
    - [Clearing the canvas](#Clearing-the-canvas)
- [Exercise 7.05: Drawing Shapes](#Exercise-7.05:-Drawing-Shapes)
- [Drawing Other Shapes](#Drawing-Other-Shapes)

[Gradients](#Gradients)

- [Exercise 7.06: Gradients](#Exercise-7.06:-Gradients)

[Animating a Canvas](#Animating-a-Canvas)

- [Exercise 7.07: Animated canvas](#Exercise-7.07:-Animated-canvas)
- [Activity 7.01: Media Page](#Activity-7.01:-Media-Page)

[Summary](#Summary)

## **Introduction**

## **Audio**

`audio`, `src`, `source`

```html
<audio controls src="media/track1.mp3">
  It looks like your browser does not support <code>audio</code>.
</audio>
```

![Getting Started](chapter7-media-audio-video-and-canvas/images/img1.png)

- ### _Exercise 7.01: Adding Audio to a Web Page_

  ![Getting Started](chapter7-media-audio-video-and-canvas/images/ex7-01.png)

- ### Attributes

  The following attributes can be used to modify the **`audio`** element

  - `autoplay`
  - `preload`
  - `loop`
  - `controls`

- #### The Autoplay Attribute

  - `controls`

- #### The preload Attribute

  - `none` The audio will not be preloaded.
  - `metadata` The browser will load audio metadata but not the whole file.
  - `auto` This is the same as an empty string; that is, `preload=""` – the whole audio file will be downloaded.

- #### The loop Attribute

  - `loop`

- #### The controls Attribute

  The `controls` attribute adds the default media controls for the browser. This allows a user to control the playback of audio. While the browser's media playback UI shares many common features (volume, mute toggle, and scrub bar, to name a few)

- ### Styling Audio Controls

  The default controls provide a lot of functionality for free. They may well be all that you need. However, as you've seen, the styles are different for each browser and may not fit with your own design or requirements. The best option for customizing the controls is to not set the `controls` attribute and to create your own custom controls with HTML, CSS, and a little bit of JavaScript.

- ### _Exercise 7.02: Styling Controls_

  ![Getting Started](chapter7-media-audio-video-and-canvas/images/ex7-02.png)

- ### Multiple Sources

  > You can learn more about media formats and browser compatibility from MDN at https://packt.live/33s2I6V

  ```html
  <audio controls>
    <source src="media/track1.webm" type="audio/webm" />
    <source src="media/track1.mp3" type="audio/mpeg" />
    <source src="media/track1.ogg" type="audio/ogg" />
    It looks like your browser does not support <code>audio</code>.
  </audio>
  ```

## **The video Element**

- ### Attributes

  - `height`
  - `width`
  - `poster`

  - #### The width and height Attributes
    The `width` and `height` attributes set the width and height of the video display area, respectively. Both values are measured in absolute pixel values – in other words, the values must be non-negative integers and they cannot be percentages.
  - #### The poster Attribute
    The `poster` attribute allows you to provide the source for an image that will be shown while the video is being downloaded. If we do not set the `poster` attribute, a blank square will appear until the first frame of the video has been downloaded, and then the first frame of the video will show in place of the poster image.

- ### _Exercise 7.03: Adding Video to a Web Page_

  ![Getting Started](chapter7-media-audio-video-and-canvas/images/ex7-03.png)

## **Limitations**

> You can learn more about various restrictions and policies from the browser vendors from a variety of sources. For example, good information about Safari and iOS can be found here: https://packt.live/2CivkDQ.
> Information on autoplay in Chrome can be found here: https://packt.live/2qrGTWH.

## **The track Element**

`track`, `media`, `source`

The following attributes let you modify a track element

- `scr`The location of the external file with the text track.
- `default` One `track` element per `media` element can be set as the default track. This attribute acts as an indication and it may be overridden by user settings (such as language).
- `kind` Specifies how the text track is supposed to be used. There are several options, including

  - `subtitles`
  - `captions`
  - `descriptions`
  - `chapters`
  - `metadata`
  - The default value is `subtitles`

- `srclang` The language of the track text; for instance
  - `en` for English
  - `fr` for French. If the track is a subtitle track, then `srclang` is required.
- `label` A human-readable title that's used to differentiate between captions and subtitles.

```html
<track src="media/track1-en.vtt" kind="subtitles" label="English subtitles" />
<track src="media/track1-sparse.vtt" kind="captions" label="Sparse captions" />
<track src="media/track1-full.vtt" kind="captions" label="Full captions" />
```

![Getting Started](chapter7-media-audio-video-and-canvas/images/img2.png)

- ### Adding Subtitles

  `Web Video Text Tracks Format (WebVTT)`, `--> string`

  ```html
  <!-- WEBVTT -->

  00:00:01.000 --> 00:00:05.000 First subtitle text <br />
  00:00:10.000 --> 00:00:25.000 Second subtitle text
  ```

- ### _Exercise 7.04: Adding Subtitles_

  ![Getting Started](chapter7-media-audio-video-and-canvas/images/ex7-04.png)

## **Images**

The approaches we will look at for embedding images in a web page are

- `img`
- `picture`
- Programmable graphics

- ### The img Element

  `img`, `alt`

  ```html
  <img src="media/poster.png" alt="HTML and CSS poster" />
  ```

- ### The picture Element

  `picture`, `type`, `mime`

  ```html
  <!-- width: 0-639px show poster-small but 800up show poster-large -->
  <picture>
    <source srcset="media/poster-small.png" media="(max-width: 639px)" />
    <source srcset="media/poster-large.png" media="(min-width: 800px)" />
    <img src="media/poster.png" alt="HTML and CSS poster" />
  </picture>
  ```

- ### Programmable Graphics

  As well as loading and embedding rasterized image files, such as `.jpeg`, `.gif`, `.png`, and `.webp`, on a web page, there are some options for creating graphics programmatically

  - `Scalable vector graphics (SVG)` is an `XML-based` format for creating vector graphics on web pages.
  - The `canvas` element gives you access to a `JavaScript` drawing API that you can use to create rasterized graphics on a web page.

- #### The svg Element

  ```xml
  <svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg" width="100" height="100">
  <circle cx="50" cy="50" r="48" fill="#4717F6" />
  <path d="M 85,50 25,75 25,25 z" fill="white" /> </svg>
  ```

  ![Getting Started](chapter7-media-audio-video-and-canvas/images/img3.png)

- #### The canvas Element

  - ##### Checking for canvas Support

    ```html
    <canvas id="canvasArea" width="320" height="240">
      Your browser does not support the <code>canvas</code> element.
    </canvas>
    ```

    ```javascript
    const canvasElement = document.getElementById('canvasArea'); if (canvasElement.getContext) {
    const context = canvasElement.getContext('2d'); // we have a context so we can draw something
    } </script>
    ```

  - ##### Drawing in canvas
  - ##### The canvas Grid

    `canvas`, `width`, `height`

    ![Getting Started](chapter7-media-audio-video-and-canvas/images/img4.png)

    > canvas coordinate system

  - ##### Drawing a Rectangle

    `fillRect`, `fillStyle`, `strokeStyle`, `lineWidth`, `StrokeRect`, `fill`, `stroke`

    ```js
    context.fillStyle = "red";
    context.fillRect(50, 50, 150, 100);
    ```

    ![Getting Started](chapter7-media-audio-video-and-canvas/images/img5.png)

    > fillRect used to draw a red rectangle on the canvas 320x240 pixels

    ```js
    context.strokeStyle = "red";
    context.lineWidth = 4;
    context.strokeRect(50, 50, 150, 100);
    ```

    ![Getting Started](chapter7-media-audio-video-and-canvas/images/img6.png)

    > strokeRect used to draw a rectangle with a border on the canvas

    ```js
    context.fillStyle = "blue";
    context.strokeStyle = "orange";
    context.lineWidth = 4;
    context.rect(50, 50, 150, 100);
    context.fill();
    context.stroke();
    ```

    ![Getting Started](chapter7-media-audio-video-and-canvas/images/img7.png)

    > Fill and stroke used to draw a rectangle with a border and fill on the canvas

  - ##### Drawing a Circle

    `arc`, `true`, `false`

    ```js
    context.fillStyle = "red";
    context.arc(50, 50, 25, 0, Math.PI * 2, false);
    context.fill();
    ```

    ![Getting Started](chapter7-media-audio-video-and-canvas/images/img8.png)

    > Fill used to draw a red circle on the canvas

  - ##### Clearing the canvas

    `clearRect`, `canvas`, `canvasElement`

    ```js
    context.clearRect(0, 0, canvasElement.width, canvasElement.height);
    ```

- ### _Exercise 7.05: Drawing Shapes_

  ![Getting Started](chapter7-media-audio-video-and-canvas/images/ex7-05.png)

- ### Drawing Other Shapes

  - `moveTo`
  - `lineTo`
  - `beginPath`

    ```js
    context.fillStyle = "yellow";
    context.beginPath();
    context.moveTo(160, 60);
    context.lineTo(220, 120);
    context.lineTo(100, 120);
    context.lineTo(160, 60);
    context.fill();
    context.beginPath();
    context.moveTo(160, 140);
    context.lineTo(220, 80);
    context.lineTo(100, 80);
    context.lineTo(160, 140);
    context.fill();
    ```

    ![Getting Started](chapter7-media-audio-video-and-canvas/images/img9.png)

    > A star shape created on the canvas with the moveTo and lineTo commands

## **Gradients**

We can create two types of gradients

- `Linear`
- `Radial`
- `createLinearGradient`
- `createRadialGradient`

  ```js
  const gradient = context.createLinearGradient(0, 0, 0, canvasElement.height);
  gradient.addColorStop(0, "white");
  gradient.addColorStop(1, "black");
  ```

  ```js
  context.fillStyle = gradient;
  context.fillRect(0, 0, canvasElement.width, canvasElement.height);
  ```

  ![Getting Started](chapter7-media-audio-video-and-canvas/images/img10.png)

  > A top to bottom linear gradient from white to black

  ```js
  const gradient = context.createLinearGradient(0, 0, canvasElement.width, 0);
  ```

  ![Getting Started](chapter7-media-audio-video-and-canvas/images/img11.png)

  > A left to right linear gradient from white to black

  ```js
  const gradient = context.createRadialGradient(
    canvasElement.width * 0.5,
    canvasElement.height * 0.5,
    1,
    canvasElement.width * 0.5,
    canvasElement.height * 0.5,
    canvasElement.width * 0.5
  );
  gradient.addColorStop(0, "white");
  gradient.addColorStop(1, "black");
  ```

  ![Getting Started](chapter7-media-audio-video-and-canvas/images/img12.png)

  > A radial gradient from white to black

- ### _Exercise 7.06: Gradients_

  ![Getting Started](chapter7-media-audio-video-and-canvas/images/ex7-06.png)

## **Animating a Canvas**

- `clearRect`
- `width`
- `height`
- `canvas`
- `canvasArea`
- `setInterval`
- `setTimer`
- `requestAnimationFrame`

  ![Getting Started](chapter7-media-audio-video-and-canvas/images/img13.png)

  ```js
  const canvasElement = document.getElementById('canvasArea');
  const context = canvasElement.getContext('2d);
  context.clearRect(0, 0, canvasElement.width, canvasElement.height);
  ```

  ```js
  function drawFrame(context) {
    // first, we clear the canvas
    context.clearRect(0, 0, canvasElement.width, canvasElement.height); // ...draw something in our canvas
    // finally, request the next frame
    requestAnimationFrame(function () {
      drawFrame(context);
    });
  }
  drawFrame(context);
  ```

- ### _Exercise 7.07: Animated canvas_

  ![Getting Started](chapter7-media-audio-video-and-canvas/images/ex7-07.png)

- ### _Activity 7.01: Media Page_

## **Summary**

<!-- CONTACT -->

## Contact

Oat Phattaraphon - [@phattaraphon_c](https://twitter.com/phattaraphon_c)
