# What is CSS?
___
**CSS** (Cascading Style Sheets) lets you make beautiful web pages, but how does it operate behind the scenes? This article teaches what CSS is and how to use it with a simple syntax example, as well as some essential terminology.
![CSS](extra.PNG)
---------
## What is CSS for?
----
***CSS*** is a language for describing how documents are shown to users, such as how they are formatted, laid out, and so on.

A document is often a text file formatted using a markup language such as HTML, but other markup languages such as SVG or XML may also be used.

When you provide a document to a user, you must transform it into a format that your audience can understand. Browsers such as Firefox, Chrome, and Edge are intended to display content graphically on a computer screen, projector, or printer, for example.

--------
## CSS syntax
------
***CSS*** is a rule-based language, which means you construct rules that describe sets of styles to be applied to certain components or groups of elements on your website. "I want the main heading of my website to be shown as huge red text," for example.

The following code demonstrates a very simple CSS rule that achieves the above-mentioned styling:

h1 {

    color: red;

    font-size: 5em;
}

A CSS stylesheet will contain many such rules, written one after the other.

h1 {

    color: red;
    font-size: 5em;
}

p {

    color: black;
}

-----
## Browser support information
-----
The state of browser support is displayed in a section called "Browser compatibility" on every MDN property page (use this to check if the property can be used on your website). The compatibility part for the CSS font-family property, for example, is shown below.

### **Browser compatibility**
![Browser compatibility](https://i.gyazo.com/fb56f5144c96458da46de17e4885d8ab.png)