###Markdown language
[Markdown](http://daringfireball.net/projects/markdown/)

In SublimeText, you can also have the full syntax finding Cheat Sheet in packages

##Man under bash
--help

###Tags and code compatibility**
www.caniuse.com

###Color picking
https://color.adobe.com/ & ColorZilla plugins

###Zebra table css

```css
tr:nth-child(2n) {
    color: yellow;
}
```
###Emmet syntax
http://docs.emmet.io/abbreviations/syntax/

htpp://docs.emmet.io/cheat-sheet

###HTML Doc
https://developer.mozilla.org/en-US/docs/Web/HTML
http://www.w3schools.com/

###Refining CSS on input types
```css
input[type="submit"]
{
   
}
```

###Round borders with CSS
border-radius

###New divs in HTML5
```html
<header>
</header>
<article>
 <section>
   <aside>
   </aside>
 </section>
 <section>
 </section>
</article>
<footer>
</footer>
```
###Relative sizes
One em is the equivalent in pixel of a character (so basically its font-size). This is useful to keep elements in relative proportion to the text.

One vw is 1% of the total height of the view port (ie, the page).

vw != % - vw is relative to the page, % to the direct parent of the element!

###After and Before pseudo attributes
```html
<span class="funny">This is the story of a man that... </span>
```

```css
  span.funny:after {
    content: ':)'
  }


span.funny:before {
  content: "\2606  ";
}
```

###Inline - Block

- An inline element has no line break before or after it, and it tolerates HTML elements next to it.
- A block element has some whitespace above and below it and does not tolerate any HTML elements next to it.
- An inline-block element is placed as an inline element (on the same line as adjacent content), but it behaves as a block element.

###Panels
```html
<fieldset>
   <legend></legend>
</fieldset>
```

###Gradients
http://www.w3schools.com/css/css3_gradients.asp

###Center elements
margin: 0 auto;


###Default position

```css
position : static;
```


###Sidebars
Use aside for sidebars

```css
position:fixed;
top:0;
left : 0;
bottom :0; /*use whole page height*/
width:200px;
```



###Style checkboxes
```html
<div class="cont">
<div class="title">
  <h1>stars<span>.css</span></h1>
</div>
<div class="stars">
<form action="">
  <input class="star star-5" id="star-5" type="radio" name="star"/>
  <label class="star star-5" for="star-5"></label>
  <input class="star star-4" id="star-4" type="radio" name="star"/>
  <label class="star star-4" for="star-4"></label>
  <input class="star star-3" id="star-3" type="radio" name="star"/>
  <label class="star star-3" for="star-3"></label>
  <input class="star star-2" id="star-2" type="radio" name="star"/>
  <label class="star star-2" for="star-2"></label>
  <input class="star star-1" id="star-1" type="radio" name="star"/>
  <label class="star star-1" for="star-1"></label>
</form>
</div>
  <p>click the stars</p>
</div>


<div class="cont">
<div class="stars">
<form action="">
  <input class="star star-5" id="star-5-2" type="radio" name="star"/>
  <label class="star star-5" for="star-5-2"></label>
  <input class="star star-4" id="star-4-2" type="radio" name="star"/>
  <label class="star star-4" for="star-4-2"></label>
  <input class="star star-3" id="star-3-2" type="radio" name="star"/>
  <label class="star star-3" for="star-3-2"></label>
  <input class="star star-2" id="star-2-2" type="radio" name="star"/>
  <label class="star star-2" for="star-2-2"></label>
  <input class="star star-1" id="star-1-2" type="radio" name="star"/>
  <label class="star star-1" for="star-1-2"></label>
  <div class="rev-box">
    <textarea class="review" col="30" name="review"></textarea>
    <label class="review" for="review">Breif Review</label>
  </div>
</form>
</div>
</div>

```

```css
@import url(http://fonts.googleapis.com/css?family=Roboto:500,100,300,700,400);
*{
  margin: 0;
  padding: 0;
  font-family: roboto;
}

body{
  background: #000;
}

.cont{
  width: 93%;
  max-width: 350px;
  text-align: center;
  margin: 4% auto;
  padding: 30px 0;
  background: #111;
  color: #EEE;
  border-radius: 5px;
  border: thin solid #444;
  overflow: hidden;
}

hr{
  margin: 20px;
  border: none;
  border-bottom: thin solid rgba(255,255,255,.1);
}

div.title{
  font-size: 2em;
}

h1 span{
  font-weight: 300;
  color: #Fd4;
}

div.stars{
  width: 270px;
  display: inline-block;
}

input.star{
  display: none;
}

label.star {
  float: right;
  padding: 10px;
  font-size: 36px;
  color: #444;
  transition: all .2s;
}

input.star:checked ~ label.star:before {
  content:'\f005';
  color: #FD4;
  transition: all .25s;
}


input.star-5:checked ~ label.star:before {
  color:#FE7;
  text-shadow: 0 0 20px #952;
}

input.star-1:checked ~ label.star:before {
  color: #F62;
}

label.star:hover{
  transform: rotate(-15deg) scale(1.3);
}

label.star:before{
  content:'\f006';
  font-family: FontAwesome;
}

.rev-box{
  overflow: hidden;
  height: 0;
  width: 100%;
  transition: all .25s;
}

textarea.review{
  background: #222;
  border: none;
  width: 100%;
  max-width: 100%;
  height: 100px;
  padding: 10px;
  box-sizing: border-box;
  color: #EEE;
}

label.review{
  display: block;
  transition:opacity .25s;
}



input.star:checked ~ .rev-box{
  height: 125px;
  overflow: visible;
}

```