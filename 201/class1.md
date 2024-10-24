# Read: Class 01

my general understanding and why this is important: knowing the basics why os java, html, and css are super important even the little things like where to start and why to start. without an idea of what it is you even wanna do is super important cause without an idea you cant really go much further. having basic knowlage of what tools you can use and how to use them are super important cause its literally the foundation of your page and you cant build a house with no foundation. the ideas and frame and critical to the end result and should be taken just as serious as the meat and final touches of not only the work we do in class but pretty much everything we do.

## how HTTP sends data between computers

## Compose a short poem describing how HTTP sends data between computers

+roses are red and violets are blue i never claimed to be a poet but heres the answer for you.. client requests something is goes to the servers and servers respond to the client and the cycle continues..

## Describe how HTML, CSS, and JS files are “parsed” in the browser

+The browser parses the HTML file first, and that leads to the browser recognizing any < link >-element references to external CSS stylesheets and any < script >-element references to scripts.
+As the browser parses the HTML, it sends requests back to the server for any CSS files it has found from < link > elements, and any JavaScript files it has found from < script > elements, and from those, then parses the CSS and JavaScript.
+The browser generates an in-memory DOM tree from the parsed HTML, generates an in-memory CSSOM structure from the parsed CSS, and compiles and executes the parsed JavaScript.
+As the browser builds the DOM tree and applies the styles from the CSSOM tree and executes the JavaScript, a visual representation of the page is painted to the screen, and the user sees the page content and can begin to interact with it.

_shortened and dumbed down_
first starts with html which ecignizes any n\links from css style sheets as well as script element references. then it sends a request back to the server for any css files its found  from the link elements or script elements (or both).. then it generates an in memor dom tree  from the parser html then generates an in memory cssom structure and compiles and executes the parsed JavaScript  then leading to a visual representation of the page thats painted to the screen.. and thats what the user will see!

## How can you find images to add to a Website?

+find an img you like or create one on your own but be sure an link the original creator 

## How do you create a String vs a Number in JavaScript?

+string -This is a sequence of text known as a string. To signify that the value is a string, enclose it in single or double quote marks.
_example_
let myVariable = 'Bob'; or
let myVariable = "Bob";
+number -This is a number. Numbers don't have quotes around them.
_example_
let myVariable = 10;

## What is a Variable and why are they important in JavaScript?

In a script, a variable declared using var is added as a non-configurable property of the global object. This means its property descriptor cannot be changed and it cannot be deleted using delete. JavaScript has automatic memory management, and it would make no sense to be able to use the delete operator on a global variable.

links used for imformation and answers are as shown

https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics
https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/What_will_your_website_look_like
https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works

## What is an HTML attribute?

+Attributes contain extra information about the element that won't appear in the content. In this example, the class attribute is an identifying name used to target the element with style information.

_An attribute should have:_

+ A space between it and the element name. (For an element with more than one attribute, the attributes should be separated by spaces too.)
+ The attribute name, followed by an equal sign.
+ An attribute value, wrapped with opening and closing quote marks.

## Describe the Anatomy of an HTMl element.

_individual elements combine to form an entire HTML page:_

< html lang="en-US" >
  < head >
    < meta charset="utf-8" / >
    < title >My test page</title>
  </head >
  < body >
    < p >This is my page</p>
  </body>
</html>

_lets go a little more in depth_
Here we have:

< !doctype html >: The doctype. When HTML was young (1991-1992), doctypes were meant to act as links to a set of rules that the HTML page had to follow to be considered good HTML. Doctypes used to look something like this:

html
Copy to Clipboard
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
More recently, the doctype is a historical artifact that needs to be included for everything else to work right. <!doctype html> is the shortest string of characters that counts as a valid doctype. That is all you need to know!

< html ></ html >: The < html > element. This element wraps all the content on the page. It is sometimes known as the root element.

< head ></head >: The < head > element. This element acts as a container for everything you want to include on the HTML page, that isn't the content the page will show to viewers. This includes keywords and a page description that would appear in search results, CSS to style content, character set declarations, and more. You will learn more about this in the next article of the series.

< meta charset="utf-8" >: The < meta > element. This element represents metadata that cannot be represented by other HTML meta-related elements, like < base >, < link >, < script >, < style > or < title >. The charset attribute specifies the character encoding for your document as UTF-8, which includes most characters from the vast majority of human written languages. With this setting, the page can now handle any textual content it might contain. There is no reason not to set this, and it can help avoid some problems later.

< title ></ title >: The < title > element. This sets the title of the page, which is the title that appears in the browser tab the page is loaded in. The page title is also used to describe the page when it is bookmarked.

< body ></body>: The < body > element. This contains all the content that displays on the page, including text, images, videos, games, playable audio tracks, or whatever else.

## What is the Difference between < article > and < section > element tags?

< article > is self-contained and can stand alone.
< section > is used for organizing content that fits into a larger context.

_article_
< article > Element
+Purpose: The < article > element is used to define a self-contained, independent piece of content that could be distributed or republished on its own (such as a blog post, news article, forum post, or product listing).
+Use Case: Think of an < article > as something that makes sense standing alone, without relying heavily on the surrounding content for context.

_example_
+< article >
  < h1 >The Benefits of Morning Exercise</h1>
  < p >Exercising in the morning can help boost your mood and energy levels for the entire day.</p>

  < p >Studies have shown that early workouts can improve concentration and mental clarity.< /p >

</article>

< section >

+Purpose: The < section > element is used to define a thematic grouping of content within a larger document. It generally groups related content under a common theme, but it's typically a part of a larger whole, rather than standalone.
+Use Case: A < section > organizes content that may be part of a broader document, like dividing an article into sections.

_example_
+< section >
  < h2 >Introduction to Web Development</h2>
  < p >Web development is the work involved in developing a website for the Internet or an intranet.</p>
</section>
< section >
  < h2 >Front-end vs Back-end</h2>
  < p >The front-end refers to the part of the website that users interact with, while the back-end refers to the server-side logic.</p>
</section>

## What Elements does a “typical” website include?

+ header
+ nav bar (links an such)
+ main content
+ side bar
+ footer

## How does metadata influence Search Engine Optimization?

+it helps search engines understand the content of a webpage and, in turn, determines how that page is ranked and displayed in search engine results pages

## How is the < meta > HTML tag used when specifying metadata?

+ to specify metadata about a web page. This metadata is not displayed on the page itself but is processed by browsers, search engines, and other services to better understand and handle the content of the page

links to pages used for answers are as follows

https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started
https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure
https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML

_extra info_
__how to start to design a webpage__

 +know what it is that you want! get an idea of what you want the webpage to look like write it down or frame it out so you dont lose sight of the rough end goal. rough draft is very important its hard to make something when you have no idea what it is you even want to create! _(project ideation)_

__most important question to answer when designing a Website?__

+what needs to be done in order to reach your goals?... have a goal and know what needs to be done to reach those goals!

Example.. i want my next page to have all working links to other simple pages (nothing fancy or crazy, i just want them to work) an for that i know i need ot make sure i make 3 other websites and publish them so that i can link them to my main website!

IE a goal and a solution to get to where i want to be.

reference page for my answer
https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML

## _semantics_

## Why should you use an < h1 > element over a < span > element to display a top level heading?

+the < h1 > element is a semantic element, which gives the text it wraps around the role (or meaning) of "a top level heading on your page."

+you can also make things look like a top level heading using < span > this will render it to look like a top level heading, but it has no semantic value, so it will not get any extra benefits.

reference page used for my answers
https://developer.mozilla.org/en-US/docs/Glossary/Semantics

_java script__

## name 2 things that require java script in the browser

+Dynamic Content Updates: JavaScript allows a web page to load new content without refreshing the entire page. For example, this is used in news feeds or live updates on social media.

+Interactive Elements: JavaScript enables features like form validation, animations, and interactive maps, enhancing user experience by responding to user actions without needing server interactions.

## How can you add JavaScript to an HTML document?

+the < script > element

reference page used for my answers

https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript
