# Snippette's walkthrough

A Snippette markdown file contains the following types of content:

```
» (optional) free form instructions how to perform the demo
» short hints for each step of the demo
» followed by a code snippet to use

Click the ">" button in top-right corner to advance.
```

You can structure your markdown any way you want, for example:

```
# My Demo Name
## Intro
... instructions ...
## Demo
... instructions ...
## Outro
... instructions ...
```

Any instructions, links, headings, etc are optional because,

```
Snippette will ignore everything that is not a code snippet 
and the sentence *before* a code snippet.

Any other content you write in the markdown is just for you: 
hints to yourself for rehearsals or to print out and 
have handy during the live demo.
```

Snippette scans your markdown for any text hints followed by a code block:

```
Append this to the `addProduct()` method:

 ```
 print(products.count)
 ```
```

During live demo you need to keep doing this:

```
» click Snippette's icon to see current hint/code
» click on the code to copy it and close the window
» paste the code in your IDE and talk to the audience
» repeat until you finished the demo
```

Where to go next?

```
Visit www.snippette.com for video walkthrough
and example markdown files for download :) 
```

