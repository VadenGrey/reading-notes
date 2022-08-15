# Class 01
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
Creating a string:
```
let x = 







*Some material copied from* [MDN](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works)
