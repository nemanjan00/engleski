layout: true
class: center, middle, inverse

---

# Web

.footnote[[Nemanja Nedeljković](https://nemanjan00.org/)]

---

## How does web work? 

---

## How does computer know where to look for website? 

---

layout: false

# Komunikacija [Računar-Server]

.left-column[
  ## DNS
]

.right-column[
  ## Protocol

  Browser: Hey, DNS root, do you know where google.com. is?

  DNS Root: No, but I know who knows where to look for. Ask com. TLD.

  Browser: Hey, com. TLD, do you know where google.com. is?

  TLD: No, but I know who knows. Ask ns1.google.com. 

  Browser: Hej, ns1.google.com., do you know where google.com. is?

  ns1.nesto.com: Yes, you can find it at 91.245.214.159

]

---

layout: true
class: center, middle, inverse

---

## Ok, now I know where to look for google, but how do I get webpage?

---

layout: false

# Komunikacija [Računar-Server]

.left-column[
  ## DNS
  ## HTTP/S
]

.right-column[
  ## Protocol

  Browser: Hey, 91.245.214.159, can you give me your index page? 

  91.245.214.159: Here you go
]

---

layout: true
class: center, middle, inverse

---

## Okay, now I have a bunch of text, but, where do I find all the images and stylesheet goodness?

---

layout: false

# Web languages [Frontend]

.left-column[

  ## HTML

]

.right-column[
  ## HTML [HyperText Markup Language]

  - HTML is language for describing page content.

  - It is made of blocks of code

  ```HTML
	<tag-name attribute1="value" attribute2=...> </tag-name>
  ```

  - Primer

  ```HTML
  <html>
	  <head>
		  <title>
			  Example
		  </title>
	  </head>
	  <body>
		  <p>paragraph</p>
	  </body>
  </html>
  ```
]

---

<img src="http://www.presse-citron.net/wordpress_prod/wp-content/uploads/IMAG04221.jpg" alt="HTML joke" style="width: 50%; margin-left: 25%;" />

---

layout: true
class: center, middle, inverse

---

## Ok, but that's just images and text now, how do I make it shine?

---

layout: false

# Web lanuages [Frontend]

.left-column[

  ## HTML
  ## CSS

]

.right-column[
  ## CSS [Cascading Style Sheets]

  - CSS is language that gives all these colors and shapes to pages [HTML]

  - Also made out of blocks

  ```CSS
  selector {property: value; property: value...}
  ```

  - Primer

  ```CSS
  body { /* Style describing body tag */
	  color: blue; /* Text is color blue */
	  background-color: red; /* Background color is red */
	  margin-top: 15px; /* Top margin is 15px */
  }
  ```
]

---

```css
.heart-shape{
    position: relative;
    width: 200px;
    height: 200px;
    -webkit-transform: rotate(45deg);
    -moz-transform: rotate(45deg);
    -ms-transform: rotate(45deg);
    -o-transform: rotate(45deg);
    transform: rotate(45deg);
    background-color: red;
}
.heart-shape:before,
.heart-shape:after{
    position: absolute;
    width: 200px;
    height: 200px;
    content: '';
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    -o-border-radius: 50%;
    border-radius: 50%;
    background-color: red;
}
.heart-shape:before{
    bottom: 0px;
    left: -100px;
}
.heart-shape:after{
    top: -100px;
    right: 0px;
}
```

---

<style>
.web {
	font-size: 150px;

	color: black;
}

.heart-shape{
	margin-left:auto;
	margin-right:auto;
	top: 200px;

    position: relative;
    width: 150px;
    height: 150px;
    -webkit-transform: rotate(45deg);
    -moz-transform: rotate(45deg);
    -ms-transform: rotate(45deg);
    -o-transform: rotate(45deg);
    transform: rotate(45deg);
    background-color: red;
}
.heart-shape:before,
.heart-shape:after{
    position: absolute;
    width: 150px;
    height: 150px;
    content: '';
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    -o-border-radius: 50%;
    border-radius: 50%;
    background-color: red;
}
.heart-shape:before{
    bottom: 0px;
    left: -75px;
}
.heart-shape:after{
    top: -75px;
    right: 0px;
}
</style>


<div class="heart-shape">>
	<p class="web">CSS</p>
</div>

---

layout: true
class: center, middle, inverse

---

## Now, let's make it go crazy and interact with us! :P

---

layout: false

# Web languages [Frontend]

.left-column[

  ## HTML
  ## CSS
  ## JavaScript

]

.right-column[
  ## JavaScript

  - JavaScript is scripting language on frontend

  - It can be found in **&lt;script&gt;** or it can be referenced by it

  ```HTML
  <script src="https://code.jquery.com/jquery-2.1.4.min.js"></script>

  <script> /* some code */ </script>
  ```

  - example

  ```javascript
  var a = 5; var b = 3;

  if(a + b != 8){
		  document.write("JavaScript is not good at math! <br>");
  }

  alert("You forgot to turn off your iron!!! ");
  ```
]

