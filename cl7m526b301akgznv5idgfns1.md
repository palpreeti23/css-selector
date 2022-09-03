## CSS Selectors


## what is CSS?
CSS stands for *Cascading Style Sheets*. CSS is a design language that makes a website look more beautiful and presentable.

CSS handles the look and feel part of a web page. Using CSS, you can control the font size of the text, color, font style, backgroundColour, layout design and much more things.

### what is CSS selectors ?
CSS selector is the first part of a CSS rule. CSS selectors are used to select element in which you want to apply CSS properties.

### **type of CSS selectors**
there are different types of CSS selectors like -
- Element Selector
- Id Selector
- Class Selector
- Universal Selector
- Group Selector
- Combinator Selector
- Attribute Selector
- Pseudo-classes and pseudo-elements


that used most commonly

### 1. Element Selector
 The element selector selects the HTML element based on element name or tag. For example - p, h1, div, span, etc.

```
h1{
      font-size : 2rem;
}
```
### 2. Id Selector
the Id selector uses the attribute of an HTML element to select a specific element. the Id of an element is unique. An Id is only use to identify one single element in our html. The Selector must start with a pound sign(#).

```
#check-button{
    width: 35%;
    font-size: 1rem;
    cursor: pointer;
}
```

### 3. Class Selector
 The class selector selects HTML elements with a specific class attribute. A class can be used to identify more than one HTML elements. The selector must start with .className.

```
.container{
    text-align: center;
    display: flex;
    flex-direction: column; 
}
```

### 4. Universal Selector
Universal selector can be used to select any and all types of element in an HTML page. This selector is useful when we want to select all the elements on the page. This is denoted by the asterisk (*).
```
*{
padding: 2rem;
margine:2rem;
}
```

### 5. Grouping Selector
 The CSS grouping selector is used to select multiple elements and style them together. To group selectors, separate each selector with a comma. For example - div, span 

```
div, span{
           color: blue;
           background-color: gray;
}
```
### 6. Attribute Selector
 This type of attribute selector is used to select all the elements that have the specified attribute and applies the CSS property to that attribute.
```
p[style] {
    background-color: #00b93e;
}
```
### 7. Combinator Selector
 A combinator is something that explains the relationship between the selectors.

-  #### Descendant Selector
. A descendant selector is made up of two or more selectors separated by white space.
Syntax: A B Example: div span will match all <span> elements that are inside a <div> element.

```
div span{
          color: blue;
}
```
- #### Child combinator
A child selector matches when an element is the child of some element. A child selector is made up of two or more selectors separated by ">".
 Syntax: A > B Example: ul > li will match all elements that are nested directly inside a
 element.

```
ol>li{
      font-weight: bold;
}
```
- #### General sibling combinator
The general sibling selector is used to select all elements that follow the first element such that both are children of the same parent.
Syntax: A ~ B Example: p ~ span will match all <span> elements that follow a <p>, immediately or not.
```
img ~ p {
   background-color: burlywood;
}
```


- #### Adjacent sibling combinator
The adjacent sibling selector is used to select an element that is directly after another specific element. Sibling elements must have the same parent element
Syntax: A + B Example: h2 + p will match the first <p> element that immediately follow an  element.

```
div + p {
  background-color: yellow;
}
```

 ### 8. Pseudo-classes and pseudo-elements
- #### Pseudo classes
A : pseudo-class is used to define a special state of an element.
For example , it can be used to style an element when a user mouses over it.

```
button:hover{
background-color: gray;
}
```
- #### Pseudo elements
The :: pseudo represent entities that are not included in HTML.
```
::placeholder{
     font-size: 10px;
}
```