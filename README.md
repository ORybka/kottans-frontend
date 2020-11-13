# <a name="top">kottans-frontend</a> :smiley_cat:

### This repo was created to record my progress in [kottans frontend course](https://github.com/kottans/frontend/blob/master/README.md).

---

## Content :feet:

---

#### General

<!-- :muscle: -->

- [x] [Git Basics](#git_basics)
- [x] [Linux CLI and Networking](#linux-cli-http)
- [x] [VCS (hello gitty), GitHub and Collaboration](#git-collaboration)

#### Front-End Basics

- [x] [Intro to HTML & CSS](#html-css-intro)
- [x] [Responsive Web Design](#html-css-responsive)
- [x] [HTML & CSS Practice](#html-css-popup)
- [x] [JavaScript Basics](#js-basics)
- [ ] [Document Object Model](#js-dom)

#### Advanced Topics

- [ ] [Building a Tiny JS World (pre-OOP)](#js-pre-oop)
- [ ] [Object oriented JS](#js-oop)
- [ ] [OOP exercise](#js-post-oop)
- [ ] [Offline Web Applications](#app-design-offline)
- [ ] [Memory pair game](#memory-pair-game)
- [ ] [Website Performance Optimization](#app-design-performance)
- [ ] [Friends App](#friends-app)

![cat](/img/cat.jpg)

---

## :point_right: <a name="git_basics">Git Basics</a>

---

Thanks to [udacity](https://www.udacity.com/course/version-control-with-git--ud123) course I felt myself a superhero.
Before I was using max 5 git commands and never truly understand the real possibilities of this system.
Moreover, I perceived it more like magic. :sparkles:
For now, I have a real picture of how it works, what I can do there and how it can help me with my projects.

### Version Control with Git :heavy_check_mark:

![git-udacity-course-1](/completed-tasks/git-basics/git-udacity-1.jpg)

### Two levels at [learngitbranching.js.org](https://learngitbranching.js.org/?locale=uk) :heavy_check_mark:

![learngitbranching-1](/completed-tasks/git-basics/learngitbranching-1.jpg)
![learngitbranching-2](/completed-tasks/git-basics/learngitbranching-2.jpg)

### Summary :smile_cat:

:zap: **Things that were new to me**

- Finally I learnt **the main definitions** of Git and I can draw in my mind where and how all the code goes;
- `$ git log` - list of commits (!don't forget to end with Q);
- file **.gitignore** - perfect way to list the files you don't them to be your repo;
- `$ git tag -a` - add tags to specific commits;
- As I am working alone now I've never faced branching and merging topics. I liked these the most. Very powerful tools, can't wait to use them for real.
  - `$ git branch <branchName>`- to create a new branch;
  - `$ git checkout <branchName>` - to switch to a specific branch;
  - `$ git checkout -b <branchName>` - to create a new branch and simultaneously switch to it;
  - `$ git rebase`- to copy commits from one branch to another;
  - `$ git merge <branchName>` - to merge a specific branch into the one where you are now;
  - **Resolving a merge conflict** - it's quite simple to do (as for now, when it's not a big project I guess :sweat_smile:);
- Commands to change/delete your commits:
  - `$ git commit --amend` - change the last commit;
  - `$ git revert <SHA>` - revert a specific commit and add new one with changes;
  - `$ git reset` - can be `--mixed`(by default), `--soft` and `--hard` (be CAREFUL);
- New commands related to the remote repo, such as:
  - `$ git fetch`
  - `$ git fakeTeamwork`
- Related commit references (was not that easy to get it but I did it :D)

:zap: **Things that surprised me**
Never used such an impostant and so informative command as `$ git log`.
Of course I liked the most `$ git log --oneline`. Little time to scroll and you have everything you need.

:zap: **Things I intend to use in the future**
I am already and will in the future use `$ git log` command as well as all the commands related to the branching and merging.
I foutd very useful command `$ git log --oneline --graph --all`.
Can't wait to see how it all works in a real project.

[:top:](#top)

---

## :point_right: <a name="linux-cli-http">Linux CLI and HTTP</a>

---

This section was informative for me, especially when it comes to networking topic, which was quite difficult to get (I tried to start reading the article for more than 5 times and ended up watching youtube videos and asking my brother for help :sweat_smile: :sweat_smile:). But I totally agree that I had to go through this.
On the other hand, I've already known most of the commands from the Linux topic, but some of them will fill up my notes.

### Linux Survival (4 modules) :heavy_check_mark:

![linux-1](/completed-tasks/task_linux_cli/linux-1.jpg)
![linux-2](/completed-tasks/task_linux_cli/linux-2.jpg)
![linux-3](/completed-tasks/task_linux_cli/linux-3.jpg)
![linux-4](/completed-tasks/task_linux_cli/linux-4.jpg)

### Summary :smile_cat:

:zap: **Things that were new to me**

**Linux CLI**

- `$ mv` - didn't know that you can use it for renaming;
- `$ pwd` to print your working directory;
- totally new staff about security and a command `$ chmod` to change those settings;
- `$ man` to open the manual and find out about a command needed;
- `$ find` - great command to find files by name, date, owner etc;
- `$ cat` - to combine files;
- commands related to a printer;
- `$ df` (disk free) - how much space you have;
- `$ ps aux` (process status) - to manage process that are already running on your computer;
- `$ grep` - to find words in files and much more.
- `/` at the start path is root, without `/` is relative;
- `~` - home directory;
- `rwx` - read write execute, `u` - user, `g` - group, `o` - world;
- `>` - overwrite, `>>` - append
- `|` - sends the output of a command as the input to another command

**HTTP**

All the topic was totally new for me and quite difficult to understand.
The main points are:

- Communication **protocol**, is a set of rules for exchanging information over a network;
- HTTP, TCP & IP are on 3 different layers (there are many more of layers):
  - application layer (HTTP/HTTPS);
  - transport layer (TCP);
  - internet layer (IP).
    **HTTP is a protocol over TCP, which is over IP**
- **HTTP** functions as a request–response protocol in the client–server computing model. In simple words, this is a language for computers.
- Communication between a host and a client occurs, via a request/response pair. The client initiates an HTTP request message, which is serviced through a HTTP response message in return. Main points here:
  - **URL** reveals the identity of the particular host with which we want to communicate;
  - **Request methods (verbs)** indicate the desired action to be performed on the identified resource. The most commonly used one is GET (other important are POST, PATCH, PUT, DELETE);
  - **Status code** tells the client how to interpret the server response: Informational `1XX`, Successful `2XX`, Redirection `3XX`, Client Error `4XX`, Server Error `5XX`.
    ![http](/img/http.jpg)
  - **General Headers** are shared by both request and response messages;
  - **Entity headers** used to provide meta-information about the the content (aka Message Body or Entity);
- **HTTPS** is a secure version of HTTP, inserting an additional layer between HTTP and TCP called TLS or SSL;
- An **HTTP cookie** is a small piece of data stored on the user's computer by the web browser while browsing a website;
- Two types of **Authentication**: _basic_ authentication is a method for an HTTP user agent to provide a user name and password when making a request and a _digest_ one which uses a more secure hashing function to encrypt the username and password.
- **HTTP Caching** is an information technology for the temporary storage (caching) of Web documents, such as Web pages, images, and other types of Web multimedia, to reduce server lag. The main advantage is that cashing csn do a freshness check to determine the age of the content in the cache; make a request to refresh the content only if necessary.

- **TCP** is a reliable transport protocol to establishe a connection between the client and server. A TCP stream is broken into IP packets, and it ensures that those packets always arrive in the correct order without fail;
- TCP uses a three-way **handshake** to establish a reliable connection.

- **IP** is the principal communications protocol for relaying datagrams across network boundaries. Its routing function enables internetworking and essentially establishes the Internet.

:zap: **Things that surprised me**

As the Networking topic was new for me, deep dive into it was quite surprising and with lots of things to think about and to analyze.

:zap: **Things I intend to use in the future**

**Linux CLI**. I think I will use most of the commands, especially those which stand for the manipulation with files and directories.

**HTTP**. I think the main purpose of this article for me at the beginner level is that it's important to know how networking works. So in the future, I will be able to communicate with server and read properly it's responses.

[:top:](#top)

---

## :point_right: <a name="git-collaboration">Git Collaboration</a>

---

This section has deepened my knowledge about Git :muscle:
And here I understood how is the process of making pull request goes.

### GitHub & Collaboration :heavy_check_mark:

![udacity-screenshot](/completed-tasks/task_git_collaboration/udacity.jpg)

### Levels at [learngitbranching.js.org](https://learngitbranching.js.org/?locale=uk) :heavy_check_mark:

![learngitbranching-3](/completed-tasks/task_git_collaboration/learngitbranching-3.jpg)
![learngitbranching-4](/completed-tasks/task_git_collaboration/learngitbranching-4.jpg)

### Summary :smile_cat:

:zap: **Things that were new to me**

- `$ git remote add origin <URL>` - to set a shortname to refer to the location of the remote repository;
- **Forking** the project -- would be totally new for me but I've experienced it while making PR to the kottan's mock repo;
- `$ git shortlog` displays an alphabetical list of names and the commit messages that go along with them:
  - `-s -n` flags to show only the number of commits each author has made, sorted numerically;
  - `$ git log --author=<name>` flag to filter the commits to the provided author(with "" for more than 1 word);
- `$ git log --grep` - to find words;
- **CONTRIBUTING.md File** - a file lists out the information you should follow to contribute to the project;
- **GitHub Issues** - the nice way to communicate back and forth with a project maintainer on code changes before starting to work on your contribution to the project;
- A **pull request** is a request to the original or source repository's maintainer to include changes in their project that you made in your fork of their project.

![git-collaboration](/img/git-col.jpg)

- **Squashing** - combining commits together with `$ git rebase -i <base>` (later use `$ git push -f origin <branch>`);
- **You should not rebase if you have already pushed the commits you want to rebase!**
- `git cherry-pick <SHA1> <SHA2> <...>` - to copy commits to the current location (HEAD);
- `$ git describe <link>`- where the result is "nearest tag_number of commits to it_SHA";
- `$ git push origin <source>:<destination>`;
- `$ git fetch origin <source>:<destination>`;
- `$ git push origin :<destination>` - to delete the branch and 0/branch;

:zap: **Things that surprised me**

To be honest I was surprised to see such a huge project as the Google one. It's great that Git has so many instruments to search for the specific information and commits, so you can work with such a huge project and don't get lost. And you can easily propose your changes by making a pull request.

:zap: **Things I intend to use in the future**

I am sure I will use all main commands, such as `git remote`, `git pull` and`git push` etc. As well as creating PR and working on big projects with other developers.

[:top:](#top)

---

## :point_right: <a name="html-css-intro">Intro to HTML & CSS</a>

---

This section had not so many new things for me but some af the materials surprised me :D
Also I liked a lot the way you can study with codecademy, very nice practical solution!

### Udacity course. Intro to HTML & CSS :heavy_check_mark:

![udacity-screenshot](/completed-tasks/task_html_css_intro/udacity.jpg)

### Codecademy course. Learn HTML :heavy_check_mark:

![codecademy-html-screenshot](/completed-tasks/task_html_css_intro/codecademy-html.jpg)

### Codecademy course. Learn CSS :heavy_check_mark:

![codecademy-css-screenshot](/completed-tasks/task_html_css_intro/codecademy-css.jpg)

### Summary :smile_cat:

:zap: **Things that were new to me**

The subject of courses was not new for me except of some details, but it was nice to refresh my knowledge about html & css, especially about:

- **Tables**. Very important to get used to their structure so you will be able to fill them in the right way, using `<tr>` for table rows and `<td>` for table data.
- **Forms**. This lesson remind me of couple of main type of input tag, such as `text`, `password`, `number`, `range`, `checkbox`, `radio` and `submit` and their attributes. Also such tag as `<datalist>`, `<textarea>` and how to make a dropdown list. It is important to write an assosiated label with some of them.

- **Form validation** topic was totally new for me.

- `<hr>` - an element that is used to a break between paragraph-level elements. It is displayed as a horizontal line.

- I will leave a note for myself here:
  - _flex-grow_ is used to specify how much space (and in what proportions) flex items absorb along the main axis.
  - _flex-shrink_ is used to specify how much flex items shrink and in what proportions along the main axis.
  - _flex-basis_ is used to specify the initial size of an element styled with flex-grow and/or flex-shrink.
  - grid-template-columns: **repeat**(3, 100px);
  - grid-template-columns: 100px **minmax**(100px, 500px) 100px;

:zap: **Things that surprised me**

These are things that were new for me and I'm surprised I didn't know that:

- **IDs are the most specific selector in CSS, followed by classes, and finally, tags.** Since IDs override class and tag styles, they should be used sparingly and only on elements that need to always appear the same.
- **Margin Collapse**. Unlike horizontal margins, **vertical margins** do not add. Instead, the larger of the two vertical margins sets the distance between adjacent elements.
- **z-index** property does not work on static elements.
- The **clear** property (which I've never used) specifies how elements should behave when they bump into each other on the page.
- **Hue, Saturation, and Lightness** for defining a color scheme.
- **word-spacing** and **letter-spacing**. It’s good to use _em_ values in this case because _em_ is dynamic — for word spacing, it sets the spacing based on the size of the font.
- `display: inline-flex` - flexbox provides the inline-flex value for the display attribute, which allows us to create flex containers that are also inline elements.
- align-items is for aligning elements within a single row. If a flex container has multiple rows of content, we can use align-content to space the rows from top to bottom.
- max-height for activating a _strech effect_;
- **grid-auto-rows** specifies the height of rows added implicitly to the grid, while **grid-auto-columns** specifies the width of columns added implicitly to the grid;
- **grid-auto-flow** specifies whether new elements should be added to rows or columns.

:zap: **Things I intend to use in the future**

From the list of new things, I will use form validation for sure.
All the materials are the basic knowledge for every Frontend developer, so for sure I will use them every day :)
And I do like the topic of flexbox and how couple of strings of your code can make such things.

[:top:](#top)

---

## :point_right: <a name="html-css-responsive">Responsive Web Design</a>

---

This section also had not so many new things for me but some af the materials surprised me a lot :D
And I did love the froggy game <3

### Udacity course. Responsive Web Design Fundamentals :heavy_check_mark:

![udacity-screenshot](/completed-tasks/task_responsive_web_design/udacity.jpg)

### Flexbox Froggy :heavy_check_mark:

![flexbox-froggy-screenshot](/completed-tasks/task_responsive_web_design/flexbox-froggy.jpg)

### Summary :smile_cat:

:zap: **Things that were new to me**

- Four types of **responsive patterns** (and their combinations):

  - mostly fluid;
  - column drop;
  - layout shifter;
  - off canvas.

- **Order for flex items**. If you want the item to becom first in the order, you have to set property order: -1;. Other items will have 1, 2, 3 so on for the order you need.

:zap: **Things that surprised me**

- **A pixel is not a pixel!** :scream: :scream:
  - **Physical pixels vs Device Independent Pixels** (simple example):
    The first iPhones had a resolution of 320×480, with a physical screen size of 3.5″. The iPhone 4 has the same physical screen size, but was the first to have a ‘Retina’ screen, with a resolution of 640×960. This was accomplished by doubling the physical pixel density; for each pixel in the screen of the iPhone 3G, both horizontally and vertically, the iPhone 4 had four.
    In order to keep compatibility with existing mobile web apps a new concept was introduced: the device-independent pixel (DIP). What this means is that the screen keeps a virtual resolution of 320×480, the same as previous screens, but for each DIP, there are four physical pixels in the same space.
  - The number of device pixels that make up a CSS pixel in one direction is its **Device Pixel Ratio (DPR)**. You can interpret this as the width (or height) of the grid of device pixels that fit inside one CSS pixel. Every device has a different _DPR_. Higher resolution devices have a higher DPR.
  - On a display with density less than 200dpi, the ratio is 1.0. On displays with density between 200 and 300dpi, the ratio is 1.5. For displays with density over 300dpi, the ratio is the integer floor(density/150dpi). Note that the default ratio is true only when the viewport scale equals 1.
    ![how-does-dpr-work](/img/dpr.jpg)
- Always remember! **Tap targets** or anyth that a user might touch, tap, click, or try do input on, need to be big enough and easy to hit. Better make 48px\*48px btns (include size and space around).
- **Ideal measure** (the length of a line of text) -> 45-90 characters per line (the best is 60cpl);

:zap: **Things I intend to use in the future**
I will use most of the concepts I learnt in the udacity course.

[:top:](#top)

---

## :point_right: <a name="html-css-popup">HTML & CSS Practice</a>

---

### Hooli-style popup :heavy_check_mark:

![hooli-screenshot](/completed-tasks/html-css-practice/hooli.jpg)

#### [Demo website](https://orybka.github.io/hooli/)

### Summary :smile_cat:

:zap: **Things that were new to me**

Going through the pull request (with files) and code review is very new for me.

I think all the process on github is made very nice.

:zap: **Things that surprised me**

I was suprised I can make a popup like that without JavaScript.

Quite an unusual and successful solution with checkboxes as for me.

:zap: **Things I intend to use in the future**

Definitely I will use my new knowledge about checkboxes in the future!

And I will pay more attention to what is written in the task :sweat_smile:

[:top:](#top)

---

## :point_right: <a name="js-basics">JavaScript Basics</a>

---

I think this part is very important for the future understanding of JavaScript as here we are getting familiar with all basics of the language.
Even though I've already completed most of the exercises at freecodecamp.org it was nice to look through them one more time and complete the one I quited last time.

### Udacity course. Intro to JavaScript :heavy_check_mark:

![udacity-js](/completed-tasks/task_js_basics/udacity-js.jpg)

### JavaScript Algorithms and Data Structures at [FreeCodeCamp](https://www.freecodecamp.org/learn/) :heavy_check_mark:

![freecodecamp](/completed-tasks/task_js_basics/freecodecamp.jpg)

### Summary :smile_cat:

:zap: **Things that were new to me**

I learnt about Functional programming and its principles for the first time. I liked this approach and hope I will be able to use it in the future.

Also it was nice to refresh the basics.

**Functional programming** is about:

1. Isolated functions - there is no dependence on the state of the program, which includes global variables that are subject to change

2. Pure functions - the same input always gives the same output

3. Functions with limited side effects - any changes, or mutations, to the state of the program outside the function are carefully controlled

A _parameter_ is always going to be a variable name and appears in the function declaration. An _argument_ is always going to be a value which appears in the code when the function is called or invoked.

**null** - "value of nothing vs **undefined** - "absence of value"

_Falsy values_ - false, null, 0, "", undefined, NaN. !!! `[]` and `{}` are _truthy_!!!

**Scope** is the part of the program where the particular identifier(e.g. variable of function) is visible and accessible. Global scope, function scope and block scope.

**Hoisting**. Before any code is executed, all func declarations are _hoisted_ to the top of their current scope (as well as variables declared inside them (only their declaration not its assignment)).

**Function Expression**: When a function is assigned to a variable. The function can be _named_, or _anonymous_.

A function that is passed into another function is called a **callback**.

:zap: **Things that surprised me**

I was surprised how difficult it was to solve algorithms tasks. I will have to come back to them in the nearest future.

:zap: **Things I intend to use in the future**

I want to use more often all the main array methods, such as:

`array.sort` - sorts the elements of an array according to the callback function. _mutats the original array!_

`array.map` - iterates over each item in an array and returns a new array containing the results of calling the callback function on each element. _without mutating the original array_

`array.filter` - filters the array, based on the function passed to it. Like map, it does this without needing to modify the original array. _without mutating the original array_

`array.slice([start[, end]])` - returns a copy of certain elements of an array. The first argument gives the index of where to begin the slice, the second is the index for where to end the slice (and it's non-inclusive). _without mutating the original array_

`array.splice` - takes arguments for the index of where to start removing items, then the number of items to remove. If the second argument is not provided, the default is to remove items through the end. _mutats the original array!_

`array1.concat(array2)` - the method is called on one, then another array is provided as the argument to concat, which is added to the end of the first array. _without mutating the original array_

`array.reduce` - terates over each item in an array and returns a single value (i.e. string, number, object, array). This is achieved via a callback function that is called on each iteration.

[:top:](#top)

---

## :point_right: <a name="js-dom">Document Object Model</a>

---

### Udacity course. JavaScript and the DOM :heavy_check_mark:

![udacity-dom](/completed-tasks/task_js_dom/udacity-dom.jpg)

### Algorithm Scripting Challenges at [FreeCodeCamp](https://www.freecodecamp.org/learn/) :heavy_check_mark:

![freecodecamp](/completed-tasks/task_js_dom/freecodecamp.jpg)

### Summary :smile_cat:

:zap: **Things that were new to me**

The **DOM** stands for "Document Object Model" and is a tree-like structure that is a representation of the HTML document, the relationship between elements, and contains the content and properties of the elements.

The DOM is:

- constructed from the browser
- is globally accessible by JavaScript code using the `document` object (just like a JavaScript object)

**Methods**:

- `.getElementById()` returns a single item;
- `.getElementsByClassName()`
- `.getElementsByTagName()`
- `.querySelector()` **returns a single element!**
- `.querySelectorAll()`

- `.createElement()`
- `.appendChild()`
- `.insertAdjacentHTML()` insert the new HTML in one of four different locations:

  - `beforebegin` – inserts the HTML text as a previous sibling
  - `afterbegin` – inserts the HTML text as the first child
  - `beforeend` – inserts the HTML text as the last child
  - `afterend` – inserts the HTML text as a following sibling

- `.removeChild()`
- `.remove()` - method removes the object from the tree it belongs to.

- `.setAttribute()` is not just for styling page elements. You can use this method to set any attribute for an element

- `.addEventListener()`
- `.removeEventListener()` => requires you to pass the **same exact** listener function to it as the one you passed to `.addEventListener()`!!
- `.preventDefault()`
- `.createDocumentFragment()`. Changes made to a DocumentFragment happen off-screen; there's no reflow and repaint cost while you build this

**Properties**:

- `.innerHTML` represents the markup of the element's content and returns a `DOMString` + updates an element, including its HTML
- `.textContent` sets or returns the text content of an element and all its descendants (completely ignores any CSS styling)
- `.innerText` gets the _visible_ text of the element
- `.firstElementChild`
- `.firstChild` - might return whitespace (if there is any) to preserve the formatting of the underlying HTML source code. Better use `.firstElementChild`
- `.parentElement` - example.`mainHeading.parentElement.removeChild(mainHeading)`
- `.style.cssText` to set multiple CSS styles at once
- `.className` returns a space-separated string of the classes.
- `.classList` returns an _DOMTokenList_ of the classes. The DOMTokenList itself is read-only, although you can modify it using the `add()`, `remove()`, `.toggle()` and `.contains()` methods.
- `.target`
- `.nodeName` => will return a capital string

`DOMContentLoaded` event => if you do have JavaScript code that needs to run as soon as possible, then you could put that code in the `<head>` and wrap it in a DOMContentLoaded event listener. This way it will run as early as possible, but not too early that the DOM isn't ready for it.

:zap: **Things that surprised me**

Main things I was surprised to know are:

- A **node** is the generic name for any type of object in the DOM hierarchy. An **element** is one specific type of node as there are many other types of nodes (text nodes, comment nodes, document nodes, etc...) (an `ELEMENT_NODE` is one particular type of node where the nodeType property has a value of `1`). An element is a specific type of node, one that can be directly specified in the HTML with an HTML tag and can have properties like an id or a class. can have children, etc...

- HTML5 defines an `HTMLCollection` which is a list of HTML Elements (not any node, only Elements). A number of properties or methods in HTML5 now return an `HTMLCollection`. While it is very similar in interface to a `nodeList`, a distinction is now made in that it only contains Elements, not any type of node.

- **_The EventTarget_** is an interface implemented by objects that can receive events and may have listeners for them.

- The _Chrome browser_ has a special `monitorEvents()` function that will let us see different events as they are occurring.

- Two functions can look the same, but live in two different places in memory. Looks can be deceiving!

- There are three different phases during the lifecycle of an event. They are:

  - the capturing phase
  - the at target phase
  - and the bubbling phase (from child up to parent)

- `performance.now()`

- **Reflow** is the process of the browser laying out the page. It happens when you first display the DOM (generally after the DOM and CSS have been loaded), and happens again every time something could change the layout. This is a fairly expensive (slow) process.

- **Repaint** happens after reflow as the browser draws the new layout to the screen. This is fairly quick, but you still want to limit how often it happens.

- JavaScript is **single-threaded** => the processing of one command at a time

- Both `.addEventListener()` and `.setTimeout()` are **Web APIs**.

- There are three parts you have to think about around the JavaScript **Event Loop**:

  - the Call Stack
  - Web APIs/the browser
  - an Event Queue

- We can use the `setTimeout()` method to help us write code that allows the browser to handle user interactions.

:zap: **Things I intend to use in the future**

[:top:](#top)

---

## :point_right: <a name="js-pre-oop">Building a Tiny JS World (pre-OOP)</a>

---

### Summary :smile_cat:

:zap: **Things that were new to me**

:zap: **Things that surprised me**

:zap: **Things I intend to use in the future**

[:top:](#top)

---

## :point_right: <a name="js-oop">Object oriented JS</a>

---

### Summary :smile_cat:

:zap: **Things that were new to me**

:zap: **Things that surprised me**

:zap: **Things I intend to use in the future**

[:top:](#top)

---

## :point_right: <a name="js-post-oop">OOP exercise</a>

---

### Summary :smile_cat:

:zap: **Things that were new to me**

:zap: **Things that surprised me**

:zap: **Things I intend to use in the future**

[:top:](#top)

---

## :point_right: <a name="app-design-offline">Offline Web Applications</a>

---

### Summary :smile_cat:

:zap: **Things that were new to me**

:zap: **Things that surprised me**

:zap: **Things I intend to use in the future**

[:top:](#top)

---

## :point_right: <a name="memory-pair-game">Memory pair game</a>

---

### Summary :smile_cat:

:zap: **Things that were new to me**

:zap: **Things that surprised me**

:zap: **Things I intend to use in the future**

[:top:](#top)

---

## :point_right: <a name="app-design-performance">Website Performance Optimization</a>

---

### Summary :smile_cat:

:zap: **Things that were new to me**

:zap: **Things that surprised me**

:zap: **Things I intend to use in the future**

[:top:](#top)

## :point_right: <a name="friends-app">Friends App</a>

---

### Summary :smile_cat:

:zap: **Things that were new to me**

:zap: **Things that surprised me**

:zap: **Things I intend to use in the future**

[:top:](#top)
