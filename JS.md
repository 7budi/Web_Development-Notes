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

Exercise:
- function Left_time(age){
  var year = (90 - age);
  var months = (year * 12);
  var weeks = (year * 52);
  var days = (year * 365);
  console.log("You have " + days + " days, " + weeks + " weeks," + months + " months left.")
}

Left_time(prompt("How old are you?"));
