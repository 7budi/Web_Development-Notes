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
	- For id document.getElementById("name") <- single element.
	- A more easier way is to use the query , document.querySelector("#name")
	- To be even more specific document.querySelector("#name h1")
	- Sometime we my have similar class name and when we do document.querySelector("#name .names") it will give us only the first one and for it to give us all the classes , document.querySelectorAll("#name")
	- document.querySelector("button").classList; will give us a list of classes that are attached to this element.
	- document.querySelector("button").classList.add("invisible")  will add a new class inside the list of classes on the element in the document.
	- document.querySelector("button").classList.remove("invisible") will do the opposite of add it will remove it.
	- document.querySelector("button").classList.toggle("invisible") will do the opposite of what already exit , if it is add it will remove it and if it is removed it will add it.  
	- document.querySelector("h1").innerHTML will give us everything inside the h1 tag even if there is another tag too while .textContent will only give the text.
	- document.querySelector("h1").attributes; will give us a list of attributes attached to this element.
	- document.querySelector("h1").getAttribute("href"); will give back the content.
	- document.querySelector("h1").setAttribute("href" , "https//www.bing.com"); will change the attribute.
	- document.querySelector("h1").addEventListener() sets up a function to be called whenever the specified event is delivered to the target. So the target in this case is document.querySelector("h1"). The addEventListener have two parameters. the first one event type like "Click", the second is a listener which is usually a javascript function.
	- if we want to know the identity of the click button we can use "this" to tell us which button is clicked.
	###  **Object**
		- is a data type that is used to store collection of keyed data.
			- EX: var object = {
				name : "1budi"
				age : 18,
				lang : ["eng","fren"] 
			 }
	### **Constructor function**
		- is a specialized function used as a blueprint to create and initialize multiple objects with the same structure and behavior.
		- EX: function exam (name , age , mark , grade, promostion){
			 this.name = name;
			 this.age = age;
			 this.mark = mark;
			 this.grade = grade;
			this.promostion = promostion;
  
			}

			var exam1 = new exam("Timmy" , 14 , 89 , "A" , "Pass");
			var exam2=new exam("Timmy" , 13,80, "C","Pass");

			console.log(exam2.mark);
	
	- Sometimes it better to use switch then if else because it is more simple and efficient.
		- EX: function clicks(){
				var button = this.innerHTML;
				switch (button) {
					case "w":
						var crash = new Audio('./sounds/crash.mp3');
						crash.play();
						break;
					case "a":
						var tom3 = new Audio('./sounds/tom-3.mp3');
						tom3.play();
						break;
					case "s":
						var tom2 = new Audio('./sounds/tom-2.mp3');
						tom2.play();
						break;
					case "d":
						var tom1 = new Audio('./sounds/tom-1.mp3');
						tom1.play();
						break;
					case "j":
						var snare = new Audio('./sounds/snare.mp3');
						snare.play();
						break;
					case "k":
						var kick = new Audio('./sounds/kick-bass.mp3');
						kick.play();
						break;
					case "l":
						var tom4 = new Audio('./sounds/tom-4.mp3');
						tom4.play();
						break;
					default:
						console.log(innerHTML);
						break;
					
						}
	- event can tell us the event that triggered the function  when using a type of event called keypress and that event got a property that tell which key is pressed.
		- EX:   document.addEventListener("keypress" ,function (event){
				sound(event.key);
				}
				)

## JQuery
- Is a feature rich JavaScript library designed to simplify HTML DOM tree traversal , manipulation, event handling and so on.
- Google CDN : <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.7.1/jquery.min.js"></script>
- In javascript if we wanted to select an element we would do so by document.querySelector("h1") and like this H1 would be selected but in jquery it done like this $("h1") this shows how jquery simplify things and makes it easier for the developer.
- it can select one or more if needed.

Exercise:
- function Left_time(age){
  var year = (90 - age);
  var months = (year * 12);
  var weeks = (year * 52);
  var days = (year * 365);
  console.log("You have " + days + " days, " + weeks + " weeks," + months + " months left.")
}

Left_time(prompt("How old are you?"));


- var drums = document.getElementsByClassName("drum");

for (var i = 0; i < drums.length; i++) {
    drums[i].addEventListener("click", clicks);
}                 <- to choose all the available clicks. 