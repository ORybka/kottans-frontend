# <a name="top">kottans-frontend</a> :smiley_cat:
### This repo was created to record my progress in [kottans frontend course](https://github.com/kottans/frontend/blob/master/README.md).

***
## Content :feet:
***

#### General
<!-- :muscle: -->

 - [x] [Git Basics](#git_basics)
 - [x] [Linux CLI and Networking](#linux-cli-http)
 - [ ] [VCS (hello gitty), GitHub and Collaboration](#git-collaboration)

#### Front-End Basics

 - [ ] [Intro to HTML & CSS](#html-css-intro)
 - [ ] [Responsive Web Design](#html-css-responsive)
 - [ ] [HTML & CSS Practice](#html-css-popup)
 - [ ] [JavaScript Basics](#js-basics)
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

 ***
 ## :point_right: <a name="git_basics">Git Basics</a>
 ***

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
 * Finally I learnt **the main definitions** of Git and I can draw in my mind where and how all the code goes;
 * `$ git log` - list of commits (!don't forget to end with Q);
 * file **.gitignore** - perfect way to list the files you don't them to be your repo;
 * `$ git tag -a` - add tags to specific commits;
 * As I am working alone now I've never faced branching and merging topics. I liked these the most. Very powerful tools, can't wait to use them for real.
   * `$ git branch <branchName>`- to create a new branch;
   * `$ git checkout <branchName>` - to switch to a specific branch;
   * `$ git checkout -b <branchName>` - to create a new branch and simultaneously switch to it;
   * `$ git rebase`- to copy commits from one branch to another;
   * `$ git merge <branchName>` - to merge a specific branch into the one where you are now;
   * **Resolving a merge conflict** - it's quite simple to do (as for now, when it's not a big project I guess :sweat_smile:);
 * Commands to change/delete your commits:
   * `$ git commit --amend` - change the last commit;
   * `$ git revert <SHA>` - revert a specific commit;
   * `$ git reset` - can be `--mixed`(by default), `--soft` and `--hard` (be CAREFUL);
 * New commands related to the remote repo, such as:
   * `$ git fetch`
   * `$ git fakeTeamwork` 
 * Related commit references (was not that easy to get it but I did it :D)

 :zap: **Things that surprised me**
 Never used such an impostant and so informative command as `$ git log`. 
 Of course I liked the most `$ git log --oneline`. Little time to scroll and you have everything you need.

 :zap: **Things I intend to use in the future**
 I am already and will in the future use `$ git log` command as well as all the commands related to the branching and merging.
 I foutd very useful command `$ git log --oneline --graph --all`.
 Can't wait to see how it all works in a real project.

 ***
 ## :point_right: <a name="linux-cli-http">Linux CLI and HTTP</a>
 ***
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
  * `$ mv` - didn't know that you can use it for renaming;
  * `$ pwd` to print your working directory;
  * totally new staff about security and a command `$ chmod` to change those settings;
  * `$ man` to open the manual and find out about a command needed;
  * `$ find` - great command to find files by name, date, owner etc;
  * `$ cat` - to combine files;
  * commands related to a printer;
  * `$ df` (disk free) - how much space you have;
  * `$ ps aux` (process status) - to manage process that  are already running on your computer;
  * `$ grep` - to find words in files and much more.
  * `/` at the start path is root, without `/` is relative;
  * `~` - home directory;
  * `rwx` - read write execute, `u` - user, `g` - group, `o` - world;
  * `>` - overwrite, `>>` - append
  * `|` - sends the output of a command as the input to another command

 **HTTP**
  All the topic was totally new for me and quite difficult to understand.
  The main points are:
  * Communication **protocol**, is a set of rules for exchanging information over a network;
  * HTTP, TCP & IP are on 3 different layers (there are many more of layers):
    1. application layer (HTTP/HTTPS);
    2. transport layer (TCP);
    3. internet layer (IP).
  **HTTP is a protocol over TCP, which is over IP**
  * **HTTP** functions as a request–response protocol in the client–server computing model. In simple words, this is a language for computers.
  * Communication between a host and a client occurs, via a request/response pair. The client initiates an HTTP request message, which is serviced through a HTTP response message in return. Main points here:
    * **URL** reveals the identity of the particular host with which we want to communicate;
    * **Request methods (verbs)** indicate the desired action to be performed on the identified resource. The most commonly used one is GET (other important are POST, PATCH, PUT, DELETE);
    *  **Status code** tells the client how to interpret the server response: Informational `1XX`, Successful `2XX`, Redirection `3XX`, Client Error `4XX`, Server Error `5XX`.
    ![http](/img/http.jpg)
    * **General Headers** are shared by both request and response messages;
    * **Entity headers** used to provide meta-information about the the content (aka Message Body or Entity);
  * **HTTPS** is a secure version of HTTP, inserting an additional layer between HTTP and TCP called TLS or SSL;
  * An **HTTP cookie** is a small piece of data stored on the user's computer by the web browser while browsing a website;
  * Two types of **Authentication**: *basic* authentication is a method for an HTTP user agent to provide a user name and password when making a request and a *digest* one which uses a more secure hashing function to encrypt the username and password.
  * **HTTP Caching** is an information technology for the temporary storage (caching) of Web documents, such as Web pages, images, and other types of Web multimedia, to reduce server lag. The main advantage is that cashing csn do a freshness check to determine the age of the content in the cache; make a request to refresh the content only if necessary.

  * **TCP** is a reliable transport protocol to establishe a connection between the client and server. A TCP stream is broken into IP packets, and it ensures that those packets always arrive in the correct order without fail;
  * TCP uses a three-way **handshake** to establish a reliable connection.

  * **IP** is the principal communications protocol for relaying datagrams across network boundaries. Its routing function enables internetworking and essentially establishes the Internet.

 :zap: **Things that surprised me**
 As the Networking topic was new for me, deep dive into it was quite surprising and with lots of things to think about and to analyze.  

 :zap: **Things I intend to use in the future**
 **Linux CLI**. I think I will use most of the commands, especially those which stand for the manipulation with files and directories.
 **HTTP**. I think the main purpose of this article for me at the beginner level is that it's important to know how networking works. So in the future, I will be able to communicate with server and read properly it's responses. 

 ***
 ## :point_right: <a name="git-collaboration">Git Collaboration</a>
 ***
 bla bla bla 
 [udacity](https://www.udacity.com/course/version-control-with-git--ud123) course 

 ### GitHub & Collaboration :heavy_check_mark:
 ![udacity-screenshot](/completed-tasks/task_git_collaboration/udacity.jpg)

 ### Two levels at [learngitbranching.js.org](https://learngitbranching.js.org/?locale=uk) :heavy_check_mark:
 ![learngitbranching-3](/completed-tasks/task_git_collaboration/learngitbranching-3.jpg)
 ![learngitbranching-4](/completed-tasks/task_git_collaboration/learngitbranching-4.jpg)

 
 ### Summary :smile_cat:
 :zap: **Things that were new to me**
 * `$ git remote add origin  <URL>` -  to set a shortname to refer to the location of the remote repository;
 * **Forking** the project -- would be totally new for me but I've experienced it while making PR to the kottan's mock repo;
 * `$ git shortlog` displays an alphabetical list of names and the commit messages that go along with them:
   * `-s -n` flags to show only the number of commits each author has made, sorted numerically;
   * `$ git log --author=<name>` flag to filter the commits to the provided author(with "" for more than 1 word);
 * `$ git log --grep` - to find words;
 * **CONTRIBUTING.md File** - a file lists out the information you should follow to contribute to the project;
 * **GitHub Issues** - the nice way to communicate back and forth with a project maintainer on code changes before starting to work on your contribution to the project;




 :zap: **Things that surprised me**

 To be honest I was suprised to see such a huge project as the Google one. It's great that Git has so many instruments to search for the specific information and commits, so you can work with such a huge project and don't get lost.

 :zap: **Things I intend to use in the future**
 
  I am sure I will use all main commands, such as `git remote`, `git pull` and`git push` etc.  

 ***
 ## :point_right: <a name="html-css-intro">Intro to HTML & CSS</a>
 ***

 
 ### Summary :smile_cat:
 :zap: **Things that were new to me**

 :zap: **Things that surprised me**

 :zap: **Things I intend to use in the future**


 ***
 ## :point_right: <a name="html-css-responsive">Responsive Web Design</a>
 ***

 
 ### Summary :smile_cat:
 :zap: **Things that were new to me**

 :zap: **Things that surprised me**

 :zap: **Things I intend to use in the future**

 ***
 ## :point_right: <a name="html-css-popup">HTML & CSS Practice</a>
 ***

 
 ### Summary :smile_cat:
 :zap: **Things that were new to me**

 :zap: **Things that surprised me**

 :zap: **Things I intend to use in the future**

 ***
 ## :point_right: <a name="js-basics">JavaScript Basics</a>
 ***

 
 ### Summary :smile_cat:
 :zap: **Things that were new to me**

 :zap: **Things that surprised me**

 :zap: **Things I intend to use in the future**

 ***
 ## :point_right: <a name="js-dom">Document Object Model</a>
 ***

 
 ### Summary :smile_cat:
 :zap: **Things that were new to me**

 :zap: **Things that surprised me**

 :zap: **Things I intend to use in the future**

  



 ## [:top:](#top)
