- [[CSS(]]Cascading Style sheets) is used to style our website , changing the plain text of HTML into a beautiful website.
- There are 3 way of adding CSS to the HTML document:
	1. Inline:This is used when we target only one element, it is not used very much.
		- EX: < html style="Background:red">< /html>
	2. Internal:This is used for one web page and can't be used when we have more than one webpage.
		- EX:< html> < head> < style> html { Background:red; }< /style > < /head> < /html>
	3. External:This is used when we have multi-page web page and the css lives entirely in a different file , this type is what is used mainly now days.
		- EX:< html> < head> < link rel="stylesheet" href="./style.css"> < /head> < /html>