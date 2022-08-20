# Class 01
The topics that I will write about on this page are important because it serves as a refresher to what i learned in code 102 and with code 201 we will be building off of this foundation set

When someone wants to access a webpage their machine(client) copies the the files from the server and displays it in whatever webbrowser they may have.

**How it happens**
1. The browser goes to the DNS server, and finds the real address of the server that the website lives on.
2. The browser sends an HTTP request message to the server, asking it to send a copy of the website to the client. This message, and all other data sent between the client and the server, is sent across your internet connection using TCP/IP.
3. If the server approves the client's request, the server sends the client a "200 OK" message, and then starts sending the website's files to the browser as a series of small chunks called data packets.
4. The browser assembles the small chunks into a complete web page and displays it to you.

Once the browser receives the first chunk of data, it can begin parsing the information received. Parsing is the step the browser takes to turn the data it receives over the network into the DOM (Document Object Model) and CSSOM (CSS Object Model), which is used by the renderer to paint a page to the screen.

Both DOM and CSSOM builds a "tree" from the HTML and CSS file to quickly see what goes where in the first 14kb.

**Adding Images**

If you want an image on your site you can find one online then reference it through:
```
<img href="webite.com">
```
or if you have thre file locally:
```
<img href="/folder/img.jpeg">
```

**Javascript Info**
A Variable is a value that is stored and can change with declaring it with "let" or cannot change by declaring it with "const"

Creating a string and number:
```
let x = "word"      //letters or numbers within quotes//
let y = 123         //numbers//
```

**Misc**
The first step in designing a website is to have an idea of what you want to create then make a wireframe of what you want your website to look like. After you have gathered your ideas and made a rough example of want you want it to be now ask yourself: "what needs to be done, and in what order to reach my goals?"

Semantics are the meaning of a piece of code what the reader can understand by its name such as:
```
<h1></h1>
```
which is "header 1", you wouldn't use a span tag because you cannot derive its meaning from just looking at it if you didn't already know what it was, which using semantics are beneficial because not only can you more easily see what the "code" is doing but so can someone else.

Adding functionality to your webiste requires JavaScript to add something like a button or prompt and to link it to website in the "code" you would write in the HTML:
```
<script src="myscript.js"></script>
```

## Things I want to know more about
why isn't the script tag in HTML self closing



*Some material copied from* [MDN](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works)

[Back to main page](https://vadengrey.github.io/reading-notes/)