javascript-best-practice [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/docdis/javascript-best-practice/issues)
========================

[![Join the chat at https://gitter.im/docdis/chat](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/docdis/chat)

A collection of JavaScript Best Practices

![Fit vs Fat](https://raw.github.com/nelsonic/javascript-best-practice/master/images/fit-vs-fat.jpg "Fit vs Fat")

Much like being in shape, 
writing *consistent*, *maintainable* and *performant* code
does not have to be "*aspiration*", its a *decision* we make
and stick to. If you see someone writing junk, share this with them! 


## Short List

1. *Use* the “**Good Parts**” (and *avoid* the “*Bad parts*”)
2. **Clear**, **Concise** and **Commented** Code
3. **Meaningful Variable Names** (Especially as Parameters)
4. *Avoid* **Global** Variables
5. Use **JSLint** to ensure your code is consistent.
6. *Always* **Unit Test** your Code (even for simple/quick fixes and one-liners)
7. *Learn* (“Real”/”Raw”) JavaScript (fundamentals) before using Libraries like JQuery/Backbone
8. Avoid Libraries/Modules/Frameworks until you *understand* them. especially when they are un-tested/documented `if(tests===false) alert(“Don’t use it!”)` 
9. **Never Commit**/Ship **Broken**/Buggy **Code** even when “PMs” Pressure You!
10. Its only “**Done**” when its “**Documented**”.

## Extra Mile

11. <del>Learn **CoffeeScript** it will Set you Free!</del>
12. Learn & Use **Patterns**
13. (Don’t be afraid to) *Critique* someone else’s code if they ignore any coding best practices (by pointing to the *specific* “guideline” that is not being followed)
14. Compile your code with **Source Maps** (to aid debugging)

My ambition is to write a *system* that *automatically* reviews ("*lints*") 
JavaScript code while you are writing it and rejects code that does 
*not adhere* to these best practices.

## Recommendations from Maintainable JavaScript

Maintainable JavaScript (Nicholas C. Zakas 2010) has *many* **practical** 
JavaScript best practices. 
I *highly recommend* you **buy & read** his **book**:
http://www.amazon.com/Maintainable-JavaScript-Nicholas-C-Zakas/dp/1449327680/


### Indentation

Indentation should be **four spaces** *not tabs*.

```javascript
// Good
if (true) {
    makePandaHappy();
}
```

### Line Length

Lines should be *no longer* than **80 characters**. 
Lines which go over 80 char should be wrapped after an operator (e.g. comma). 
The **continuation** line should be *indented* **two levels** (8 chars).

```javascript
// Good
registerNewUser(firstName, lastName, emailAddress, password,
        preferredLanguage);

// Bad: Continuation line only indented four spaces
registerNewUser(firstName, lastName, emailAddress, password,
    preferredLanguage);

registerNewUser(firstName, lastName, emailAddress, password
        , preferredLanguage);
```
**Note**: there are plenty of advoctes for "Leading Comma" or "Trailing Comma"
see: http://www.sencha.com/forum/showthread.php?6796-Leading-comma-or-Trailing-comma-that-is-the-question.

### Primitive Literals

#### Strings

Always use double quotes and span a single line.

```javascript
// Good
var message = "Welcome to JayessVille!";

// Bad: Single Quotes
var message = 'single quotes confuse. avoid';
```




## Recommended Reading

![Best Teachers](https://pbs.twimg.com/media/BIOLrIVCIAA7NJG.jpg:medium "Best Teachers")

Completely **New to JavaScript**? Welcome! **Start** with *this book*:

- **Dom Scripting**: Web Design with JavaScript and the Document Object Model - 
www.amazon.com/dp/B004VH7LQE  *BUY IT*! Invest in knowing how to build the future! 
(if you cannot afford the $18 for a secondhand “like new” copy, get in touch, 
I will lend it to you!) 

If you are familiar with JavaScript and not yet read “The Good Parts” start!

- JavaScript **The Good Parts** (Douglas Crockford 2008): 
http://www.amazon.com/JavaScript-Good-Parts-Douglas-Crockford/dp/0596517742/

Once you have *mastered* the **Good Parts**, *hone* your **craft**:

- JavaScript **Patterns** (Stoyan Stefanov 2010): 
http://www.amazon.com/dp/0596806752/

- Learning JavaScript **Design Patterns** (Andy Osmani 2012):
http://www.amazon.com/Learning-JavaScript-Design-Patterns-Osmani/dp/1449331815/

Now that you know the language its time for **Test Driven Development**!

- **Test-Driven** JavaScript Development (Christian Johansen, 2010):
http://www.amazon.com//dp/0321683919/  

- **Testable** JavaScript (Mark Ethan Trostler 2013): 
http://www.amazon.com/dp/1449323391/

And/or **Behaviour-Driven Development** (BDD):

- JavaScript Testing with **Jasmine**: JavaScript Behavior-Driven Development
(Evan Hahn 2013): www.amazon.com/dp/1449356370/


Time to Optimize your JavaScript? (Or looking for some simple wins?)

- **High Performance** JavaScript (Nicholas C. Zakas 2010):
http://www.amazon.com/dp/059680279X/

## CoffeeScript

I am a *huge fan* of CoffeeScript's elegance and simplicity.
But its not as popular as I would have liked. :-(

![Easy to Write Hard to Read](http://i.imgur.com/usNKZRt.png "CoffeeScript Discussion")

I actually find CoffeeScript incredibly *easy* to read (*practice*?) but I *agree*
with [@pgte](https://github.com/pgte) its harder to get contributions from others
for open source projects if they are written in CoffeeScript, simply because not
that many people know the language! :-(

I still recommend you *learn* coffeescript, its *so* **much** more fun to write
and (with *practice*) read than JavaScript! And for small teams where everyone
learns it, CoffeeScript wipes the floor with JavaScript!

### Further discussion: 
- http://net.tutsplus.com/articles/interviews/should-you-learn-coffeescript/
- http://stackoverflow.com/questions/2954557/has-anyone-used-coffeescript-for-a-production-application
- https://tech.dropbox.com/2012/09/dropbox-dives-into-coffeescript/

- **Why** CoffeeScript? http://vimeo.com/35258313
- **Try** CoffeeScript: http://coffeescript.org/ [click *Try*]
- **REPL**: http://repl.it/languages/CoffeeScript
- **Intro**: http://youtu.be/QgqVh_KpVKY 

### Book

The **Little Book** on CoffeeScript: http://www.amazon.com/dp/1449321054/
Available **FREE** at: http://arcturo.github.io/library/coffeescript/index.html

### Learn By Doing

Learn CoffeeScript by Testing with the “**Koans**”: 
https://github.com/sleepyfox/coffeescript-koans 


## Small Stack of Best Books

While I'm a **strong advocate** of **learning by doing**, 
*sometimes* it *pays* to learn from the knowledge/mistakes of
more experienced people by reading the books they have written...

I keep a *small stack* of the best titles on my desk to recommend to my
"*junior*" developers:

![Stack of JavaScript Books](https://pbs.twimg.com/media/BHfMcdNCEAAFuj0.jpg "Do your Homework")

If you live in London and can't afford to buy books, message me on 
[LinkedIn](http://uk.linkedin.com/in/nelsonic),
I'm happy to *give* you any of my books in exchange for *insights*. :-)


### Test Driven Development - Writing Reliable Code

If you are not doing Test Driven Development (TDD), you officially an ammateur; go do your *homework*!
But seriously, testing is *easy* and will give you *confidence* in the code you have written. 

Writing comprehensive tests allows you to refactor your code as you learn how to do things more efficiently (natural progression - you’re meant to keep learning; honing your craft!) and can build on your existing codebase without fear of breaking existing (decoupled) modules.

There are a wide range of options for testing JavaScript:
See: http://stackoverflow.com/questions/300855/looking-for-a-better-javascript-unit-test-tool 

I recommend reading http://www.amazon.com/dp/0321683919/ and http://www.amazon.com/dp/1449323391/ to get a good understanding of the available options.

I have used:
- Vows: http://vowsjs.org/
- Mocha: http://visionmedia.github.io/mocha/
- Jasmine: http://pivotal.github.io/jasmine/
- Chai: http://chaijs.com/ 
- JS-Test-Driver: https://code.google.com/p/js-test-driver/
- NodeJS Assert (core module): http://nodejs.org/api/assert.html 

And of these I favor Jasmine for its Simplicity. (but always keep open mind if someone has experience of others)

#### Jasmine

- Background: https://github.com/pivotal/jasmine/wiki/Background
- Try: http://tryjasmine.com/?
- Tutorial: http://net.tutsplus.com/tutorials/javascript-ajax/testing-your-javascript-with-jasmine/
- More: https://github.com/pivotal/jasmine/wiki/Suites-and-specs
- Dowload: http://pivotal.github.com/jasmine/download.html
- GitHub repo: https://github.com/pivotal/jasmine
- Using Jasmine in Node.js (server side) https://github.com/mhevery/jasmine-node
- Another good tutorial: http://evanhahn.com/?p=181




### Notes

#### Sources

- http://www.w3.org/wiki/JavaScript_best_practices 
- https://github.com/stevekwan/best-practices/blob/master/javascript/best-practices.md
- http://www.developerdrive.com/2011/08/top-10-must-follow-javascript-best-practices-2/
- http://www.codeproject.com/Articles/580165/JavaScript-Best-Practice
- http://www.javascripttoolbox.com/bestpractices/
- http://google-styleguide.googlecode.com/svn/trunk/javascriptguide.xml 
- http://net.tutsplus.com/tutorials/javascript-ajax/24-javascript-best-practices-for-beginners/



### History

This originally started out in a Google Doc:
https://docs.google.com/document/d/1t9msoVNY5KlRnHeIAgUgqDyaXh2Q35v5zHtdpZ2vy-U
I created it to share/suggest best practices with my team of developers.
The idea was that all developers in the company could edit the doc and a 
generally agreed code for writing code could be established.

The *reality* was that I was the only one who even *looked* at the Google Doc!
Nobody made any comments or contributions. :-(
*Too "Busy"* coding to stop and think: "*Is my code consistent...?*" or 
"*Is this maintainable by someone else?*" ... This is not the time or place 
to voice my *frustration* at trying to get people in an established 
organisation (with more **bad habits** than you can *imagine*) to adopt 
industry best practices for JavaScript code. 
Each to their own. 

Its time to put this up on GitHub for a wider audience to access. ;-)
