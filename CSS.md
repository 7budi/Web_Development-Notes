- [[CSS(]]Cascading Style sheets) is used to style our website , changing the plain text of HTML into a beautiful website.
- There are 3 way of adding CSS to the HTML document:
	1. Inline:This is used when we target only one element, it is not used very much.
		- EX: < html style="Background:red">< /html>
	2. Internal:This is used for one web page and can't be used when we have more than one webpage.
		- EX:< html> < head> < style> html { Background:red; }< /style > < /head> < /html>
	3. External:This is used when we have multi-page web page and the css lives entirely in a different file , this type is what is used mainly now days.
		- EX:< html> < head> < link rel="stylesheet" href="./style.css"> < /head> < /html>
- Then in another file there will be CSS selector " h1 { color:red; }".
- CSS selector helps us to select part of the html to apply which ever rule we want inside the curly braces.
- There is also Class selector which use the class attribute to help us group elements and apply the same rule to all of them.
		Ex:< p class="redT">red< /p>
- ID selector is another attribute with the same effect to class selector but the difference is that ID selector is for one element or that and it is unique while the class selector can be used for many.
		Ex:< p Id="main">red< /p>

## Font Properties
### Font size
- If we want to change the font size we can do it in different way.
	1. 1px = 1/96th inch
	2. 1pt = 1/72 inch
	3. 1em = 100% of the parent 
	4. 1rem = 100% of the root(html)
### Font weight 
- Font weight changes it just make the font a bit heavier.
1. Font-weight: bold
2. Font-weight: normal
### Font Family
- This determines how the font looks like.
	1. font-family:"New times roman", serif
	2. font-family:Helvetica, sans-serif
## The Box Model
- Margin , Padding and Border together with width and height makes the concept of the box model.
	1. Border as its name is the outer line of the box which we can adjust as much as we like.
		- EX: border:thickness style color
	2. Padding: this pushes the border by the given amount
		- EX: padding:20px;
	3. Margin:The distant between any content and the border is margin.
		- Ex:margin:10px;


## The Cascading part of CSS

 - What happen when two or three CSS rule are add to the same Element?
	 - As its name suggest it goes in sequence from the higher to the lower and the end result that will show is the last one.
	 - The first level comes from the external then internal lastly inline.
- Level of importance in CSS:
	- Position: Whether the rule is higher or lower relative to other rules.
	- Specificity: refers to how specific is a rule in terms of the element you are applying the rule to.
		1. Element
		2. Class
		3. Attribute
		4. Id <- the most specific
	- Type:
		1. External
		2. internal
		3. inline
	- Importance: this is an attribute you add to make it more important
		- EX: color: red !important;
## Positioning 
- This will help us to position our thing properly and there are 4 types of postioning:
		1. Static : This type is the HTML default.
		2. Relative: This is relative to default position.
		3. Absolute: Position relative to nearest positioned ancestor or top left corner of webpage.
		4. Fixed: Position relative to top left corner of browser window.

## CSS Display
- There are 3 commonly used display values for the display property.	
	1. Block: When this value is used it take the entire width of the block.
	2. inline: In inline case the block will default to the content width and height and connot be changed.
	3. inline-block: Inline-block allow us to change the width and the height of the block and can be in the same line with other inline or block.
## CSS Float
- Using the float element we can wrap a test with around another element.
- 