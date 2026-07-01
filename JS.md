- JavaScript is a high-level, dynamic programming language that serves as one of the core technologies of the World Wide Web, alongside HTML and CSS.
- alert is used print or op up what's wanted.
	- alert("Hello World") will show Hello world.
- prompt ask for input
	- prompt("What is your name?");
- var is a container that we put thing to save it to memory.
	- var Myname = "7budi";
- If we want to know the count or length of something we can use .length.
	- var Myname = "7budi";
	- Myname.length;
- If we want to cut or slice from a range of characters we use .slice.
	- var Myname = "7budi";
	- Myname.slice(0,3);
- To change every thing in the string to upper case we use .toUpperCase() and to change to lower case .toLowerCase().
	- var Myname = "7budi";
	- Myname.toUpperCase();
	- Myname = Myname.toUpperCase(); <- to make sure that its saved
	- ![[name.png]]
- To create a function we use function name().
	- function work(){};
- Console.log is something that will show on the console and for the developer only while alert is for the user.
- To round down a number we can use the Math.floor().
- To do a root use Math.pow(87 , 2)
- To round a number to nearest integer use Math.round().
- For random number generation Math.random() and the number that get generated is a 16 decimal place.
- Creating an control statement is done by if else.
	- if (condition === condition){
	 } else {
	 }
- Even though both == and === checks for equality the === also checks the data type.
- To create an array use, var name = \[ names].
- name.length\[ 0] counts the names inside  which is 1.
- name.include(names) will check if the item exist inside the array.
- name.push(1) will push or append to the end of the list and egg.pop will romove the last item.

## Integrating JavaScript
- There are 3 ways to add javascript to our website 
	1. Just like the CSS there is an inline were we add it to the element.
		- < body onload="alert('hello')">
	2. Internal where we have an alement called script.
		- < script>
		 alert("hello")
		 < /script>
	3. The last one will be external which is a little different form the css because in css the link tag is written in the head element so that it does the css first where as the javascript is written down right before the body closing tag so that it does everything in the end.
		- < script src="main.js">< /script>

## Document Object Model
- It is a programming interface that treats HTML page as a tree like structure of objects, this structure allow javascript to dynamically change or control the structure of a website.
- Typing document in the console will give you the entire HTML file.
- Our objects inside the DOM can have Properties and Methods.
	- Properties describe something about the Object.
		- name.color <-get property 
		- name.father = "text"; <- set property
	- Methods are the thing the object can do.
		- name.come(); <- call a Method
	- example : document.firstElementChild.lastElementChild.lastElementChild.lastElementChild.innerHTML = "HI";
	- To be more specific use document.getElementsByTagName("li")\[2].style.color = "red";
	- It can be done in this way too document.getElementsByTagName("li").length.
	- For class it can be done like this document.getElementsByClassName("text").

Exercise:
- function Left_time(age){
  var year = (90 - age);
  var months = (year * 12);
  var weeks = (year * 52);
  var days = (year * 365);
  console.log("You have " + days + " days, " + weeks + " weeks," + months + " months left.")
}

Left_time(prompt("How old are you?"));
