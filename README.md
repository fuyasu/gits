<!DOCTYPE html>
<html>
<head>
   <title>Css key point</title>
</head>
<body style="background-color: rgb(220, 220, 220);" >
<style>
h3{
  color: lightgreen;
  text-align:center;
  font-weight:;
  font-size: 30px;
  }
  
  </style>
<h1 style="color:green;" >CSS THEORY</h1>
<h3>What is css</h3>

<pre>
    CSS stands for 'Cascading Style Sheets' created by the World Wide Web Consortium. CSS is used for styling an HTML document. It defines how our web pages will look, webpage's design and layout. 
    We hope that you are familiar with HTML before learning CSS. We suggest you to use Visual Studio Code for writing CSS documents.
</pre>
<br>
<h3>What are Comments in css </h3>
<pre>
   	Comments are used as a tool which provides description of the code. Generally, comments do not have a meaning to the compiler and are ignored by it. We write comments with our code to provide an explanation of the code for future references which will help future coders to understand the code. It is a good practice to write comments. 

   	In CSS, we use forward-slash & an asterisk <code>'/*'</code> at the beginning of the comment and an asterisk & a forward-slash <code>'*/'</code> at the end of the comment. 

   	For example: 
   	/* 
	This is a comment, it will not be executed by the code compiler 
	*/ 

	Note: In this app, we'll be sharing the explanation of code mostly in comments, so make sure to read comments too. 

	Whereas in HTML, the opening tag is <code>*/ (less than, exclamation, double hyphens) and closing tag is */ </code>(double hyphens, greater than sign). Our HTML comments are written inside these tags. 

	For example: 
<code>
	*/
	This is HTML Comment 
	*/
</code>

	Throughout this app, we'll be using both types of comments in their places, so don't get confused.
<br>
<h3>Explain syntax of any css element.</h3>
</pre>
<pre>A CSS has to follow certain style rule which are described below: 
(i) Selector 
(ii) Declaration 
		(ii.a) Property 
		(ii.b) Value 

Selector- 
	A selector is an HTML element tag at which CSS will be applied. Now, you can select on whichever tag you want to apply your CSS style like h1, p etc. 

Declaration- 
	Declaration is where we define our style. A selector can have multiple declarations. It consists of property and value. 
	Property is like an attribute for the selector and we assign some value to it. 

	For example- 
!DOCTYPE html 
 html 
 head 
title This is document title /title 
 style 
h1 { 
color: black; 
} 
style 
/head 
/html 

-- In CSS, we use curly braces {} instead of triangular brackets which is used in HTML 
-- Here, h1 is the selector 
-- color is the property 
-- and black is the value assigned to the property 
-- Also note that all CSS elements are written inside the style tag.
 </pre>
 <h3>What are selectors?</h3>
 <pre>
 Selectors allows us to select the content on the webpage which we want to style. The content is the data which is wrapped inside HTML element tags. Basically, Selector allows us to select certain portions of our webpage and gives us the ability to style that portion. 
  
  Now, selection can be done in multiple ways through Selector: 
  (i) Element Selector 
  (ii) ID Selector 
  (iii) Class Selector 
  (iv) Group Selector 
  (v) Universal Selector
  
  <h3>What is an element selector?</h3>
  In Element Selector, the selection is done on the basis of the HTML element's name. 
  
  For example: 
   !DOCTYPE html 
   html 
   head 
  
   style 
  p{ 
  text-align: center; 
  color: orange; 
  } 
  /* Here, all paragraph elements will now have orange text color 
  and will be center aligned */ 
   /style 
   /head 
  
   body 
  p My 1st Paragraph /p 
  p My 2nd Paragraph /p 
  /body 
  /html
  <h3>What is an ID selector?</h3>
  In HTML elements, we can assign a unique ID to them as an attribute. So, we can use these ID's to apply CSS styling to only those particular elements. We use hash character '#' and then ID value to make the selection. 
  
  For example: 
  <code>
   !DOCTYPE html 
   html 
   head 
  
   style 
  #2{ 
  text-align: center; 
  color: orange; 
  } 
   /style 
   /head 
  
   body 
   p My 1st Paragraph /p 
  (p id="2") My 2nd Paragraph /p)
   /body 
   /html
  /* Here, only paragraph element which has an ID value of 2, 
  will have orange text color and will be center aligned */
  </code>
  
  <h3>What is class selector?</h3>
  In Class Selector, the styling will only be applied to those elements which has a specific class attribute applied to them. To make a class selector, we use a dot character '.' (also known as period character) and then followed by the class name. 
  
  For example- 
   !DOCTYPE html 
   html 
   head 
  
   style 
  .right{ 
  text-align: right; 
  color: orange; 
  } 
  .left{ 
  text-align: left; 
  color: green; 
  } 
   /style 
   /head 
  
   body 
   p class="right">My 1st Paragraph /p
   p class="left" My 2nd Paragraph /p 
   /body  
   /html 
  /* Here, the elements having class value 'right' will have text aligned in right with orange font 
  whereas, the elements having class value left will have text aligned in left with green font */
 
 <h3>What is the Group selector?</h3>
 In Group Selector, we can have the same styling applied to different types of elements in the form of group. We use group selector, only when we want to have the same type of styling in different elements, it helps us to reduce code length and complexity which makes it easier to maintain the webpage. 
 
 For example, 
 !DOCTYPE html 
  html  
  head 
 
  style 
 h1, h2, p{ 
 text-align: center; 
 color: red; 
 } 
  /style 
  /head   
 
  body 
  h1 CSS For Beginners /h1 
  h2 Tutorial App for Beginners /h2 
  p Learn CSS Basics /p 
  /body
  /html 
 /* Here h1, h2 and p tags will have same text alignment and text color as well */
 
 <h3>What is the Universal selector?</h3>
 
 In Universal Selector, the styling is applied to each and every HTML element used in the web-page. We use an asterisk '*' to apply a universal selector to all elements. The use of Universal Selector is very less in an actual website. 
 
 For example, 
  !DOCTYPE html
  html 
  head 
 
  style 
 * { 
 text-align: center; 
 color: red; 
 } 
  /style 
  /head 
 
  body 
  h1 CSS For Beginners /h1 
  h2 Tutorial App for Beginners /h2
  p Learn CSS Basics /p 
  /body  
  /html 
 /* Here, all elements like h1, h2 and p will have center alignment and font in red color */
 
 <h3>How to add css to web pages?</h3>
 The styling of any webpage is done through the information stored in the stylesheet document. Web browsers read this stylesheet to make the necessary changes on the styling of a webpage. 
 
 There are 3 ways in which we can insert CSS into our web pages: 
 (i) Inline CSS 
 (ii) Internal CSS 
 (iii) External CSS
 
 <h3>What is Inline CSS</h3>
 In Inline CSS, we apply CSS code to each element in a single line. This is useful when we want to provide different styling to each element of a webpage. To apply Inline CSS, we use style attributes with our elements tag. 
 
 For example: 
  !DOCTYPE html 
  html 
  body 
  h1 style="color:red; text-align:center;" My Website /h1 
  p style="color:blue;" CSS is good /p 
  /body 
  /html 
 
 But the downside of an Inline CSS is that it loses its stylesheet advantage.
 
 <h3>What is Internal CSS?</h3>
 In Internal CSS, we apply our CSS styling in the head section of the web page. We use Internal CSS, when we want to apply styling to only one page out of many pages of the website. All styling of Internal CSS is done inside of the  style element. 
 
 For example: 
  !DOCTYPE html 
  html 
  head 
 
  style 
 h1{ 
 color:red; 
 text-align:center; 
 } 
 p{ 
 color:blue; 
 } 
  /style 
  /head 
 
  body 
  h1 My Website /h1 
  p CSS is good /p  
  /body 
  /html
 
 /* Here, styling is done inside of the webpage but in a style element tag and not inside of the elements like in Inline CSS */
 
 <h3>What is External CSS?</h3>
 In External CSS, we can apply the same styling to multiple web pages or even on the entire website. All the styling code is written inside a CSS file with .css extension which is linked with each and every webpage of the website by using a link element inside the head of the HTML document. The advantage of using an external css styling file is that we can change the look and feel of the entire website just by changing one file. 
 
 For example: 
  !DOCTYPE html 
  html 
  head 
 
 link rel=stylesheet type=text/css href=style.css> 
 /* Here, 'rel' is relationship that the HTML document has with the CSS file 
 'type' attribute tells what kind of file it is 
 'href' contains the location of the CSS file*/ 
  /head 
 
  body 
  h1 My Website /h1 
   p CSS is good /p 
  /body 
  /html
 /* This was our HTML document, 
 the code of CSS is shared below which must be stored in a different CSS file */ 
 
 (style.css) 
 h1{ 
 	color:red; 
 	text-align:center; 
 } 
 p{ 
 	color:blue; 
 } 
 
 <h3>How to set Color in CSS?</h3>
 In CSS, we can apply colors to texts and background elements of an HTML document by using the 'color' keyword. After the color keyword, we pass a value to it. 
 
 Now, there are multiple formats in which a value for color can be specified. The color formats are: 
 (i) HEX Code 
 (ii) Short HEX Code 
 (iii) Keyword Color 
 (iv) RGB 
 
 Out of all these color formats, the most commonly used are HEX Codes.
 
 <h3>What are short hex code</h3>
 HEX Code stands for Hexadecimal Code. As the name suggests it is a 6 digit color representation. 
 
 Example of HEX Code: 
 color: #000000 
 
 Here, this is the HEX code for black. A HEX code starts with a hash symbol(#) which is then followed by a 6 digit alpha-numeric code. In HEX code, the first two digits represent red color value(RR), the middle two digits represent green color (GG) and the last two digits represent blue color value. The easy way to remember HEX code is by using ‘RRGGBB’. The value of each color ranges from 00 to 99, so we can also create our own colors by changing these values.
 
 <h3>What are short HEX codes?</h3>
 Short HEX Code as the name suggests is the short form of Hexadecimal Color Notation. 
 
 Example of Short HEX Code: 
 color: #345 
 
 Here, each digit is recreated to arrive at an equivalent hexadecimal value, which means #345 is equivalent to #334455.
 
 <h3>What are keyword colors?</h3>
 Keyword Colors are colors which are built-in in CSS. We can access these colors just with their names. They have fixed color codes assigned to them. 
 
 Examples of Keyword Color: 
 color: red; 
 color: Tomato; 
 
 Generally, we don't use these colors in
 production as we want to have more
 freedom while deciding our colors
 according to the theme of the website. 
 These colors are mostly suitable for testing purposes.
 
 <h3>What are RGB colors?</h3>
 RGB stands for Red Green Blue which are the 3 major colors we use in combination to create other colors. In RGB, each color has a range of 0 to 255. The value of RGB is specified in rgb() property. In this property, all 3 colors values are stored which can be in percentage as well. 
 
 Example of RGB: 
 color: rgb(255, 53, 76); 
 
 There is another format which is known as RGBA,
 which is very similar to RGB, but A stands for Alpha, 
 which defines the transparency of the color.
 The value of alpha is between 0.0 to 1.0, 
 in which 0.0 is used to make 
 color fully transparent and 1.0 to make solid color. 
 
 Example of RGBA: 
 color: rgb(255, 53, 76, 0.8);
 
 <h3>What are the difference between Block and Inline Elements?</h3>
 The Block Elements are those elements which take all the width present in their path as they start from a new line. 
 Some examples of Block Elements are: all headings h1 - h6, paragraph, division etc. 
 Whereas,
 the Inline Elements only takes the space 
 which is required by them. Some examples of Inline Elements are: 
 image, span, anchor. 
 But by using the Display Property, 
 we can alter the properties of block elements
 to inline and vice versa, 
 which means block elements can be set-up in a single line, 
 also inline elements can also be set-up in new lines.
  (for reference check Display Code in Codes Section)
  

 </pre>
 </body>
 </html>
