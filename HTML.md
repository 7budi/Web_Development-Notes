- [[HTML]](Hyper Text Markup Language) defines the content and the structure of the website.
- The hypertext can be said to be the texts that link to other document in the website.
- The markup language can be said to be how to structure is write ex: Bold, italic, align, space etc.

**Q1) How to Markup the HTML?**
- That is done through the HTML Tags.
- There are many Tags which we will see one by one.
## The Heading Element
 - < h1> is the opening tag.
 - < /h1> is the closing tab.
 - And the thing written in between is content.
 
 EX: < h6> Hello World < /h6>
All together is called the **Heading Element**.

## Element

1. < p> < /p> , This tag is for writing paragraph(plain text).
2. < hr /> ,This is a horizontal rule that draws a line and it doesn't need closing tag that's why it is called a void element.
3. < br />, This is a break line it can separate(break) a paragraph into one or more lines.
4. < ul> < /ul> , This is unordered list where we put a bunch of < li>< /li> list that we don't care about its order.
5. < ol>< /ol> , This is ordered list where we have to add a < li>< /li> inside but we care about the order we can add an attribute called start where we can choose from which number to start from.
6. < a> < /a>, This is called anchor element which helps us to make a hyper link through one of it's attribute EX: ( a href <-  attribute) and this attributes needs a value ( a href ="www.gogle.com" <- value) you can also add another attribute too if need.
7. < img >, This is an image element it is used to add image or pictures to the website and it need an attribute called src where it goes to the place where the image exist and pick it up, And we can add another attribute called alt where we write what the picture is about so that when someone with disability come he can click the img and it tells what the picture is about.

## File Path

- A File Path is the address or set of directions used by a browser or server to locate a specific file within a website's folder structure.
EX: C:/Example1/Example2/Example3 in window we can move to any folder.  

Like the example we can do the same in websites ./Project/img or  ../img.

Absolute path file: This is where we have to start from the start of the folder or the root folder.
Relative path file: This is when you start from your current path to the destination.

## HTML Boilerplate

- It is what we start with when we create a new html file and it looks like this:

< !DOCTYPE html> <- This tells any browser what version of html is written in.
< html lang="en"> <- everything we want to do to our website will go inside here
< head> 
- This where important information about our website is placed that is not displayed to the user.
- One thing that is placed here always the meta tag, < meta charset="UTF-8"> this insures that the characters that you use get displayed correctly.
- Another tag that should be in the head element is < Title>.
< /head>

< body>
- This is where majority of the contents goes, < p>, < a> , < img> .. etc.
< /body>

< /html> 