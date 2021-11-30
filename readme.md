# Wikipedia Preview-Box
Automatically turns any ordinary link to a Wikipedia article on your website into a link with a nice preview box (article summary). You just need to insert one line of code. Tried to make it in a way so everybody can use it.

## Example
Go to the [project page](https://su-pa.net/wikiPrevBox/) and ["Try it out"](https://su-pa.net/wikiPrevBox/).

## Features & characteristics
- Lightweight, just 109 lines of JavaScript code, some CSS, a Wikipedia logo, a font and a bullet-gif
- No installation needed: Insert one line of code and it works
- It's like magic, paste a link to a Wikipedia article in your content and the preview box just pops up!
- Works with touch & mouse, on mobile & desktop
- Preview box finds automatically the best place to display on mobile & desktop, landscape & portrait mode
- The locations of Wikipedia links that have preview boxes are visibly marked through a little Wikipedia logo (W) within the content
- Fine animation of the preview box 
- Works with all languages & mixed content
- Integrated "auto hyphenation" (CSS) for all (available) languages
- Shows summery & image (if any) inside every preview box (default)\
Possible settings:
  - Show inside all preview boxes only the summary text, no images
  - ... as before, but nevertheless show the image for a specific Wikipedia links
  - Deactivate the preview box for a specific link
  - Vary the width of the preview boxes
- Easy using settings
- Simple to use on any website, web app or to [integrate in WordPress](https://su-pa.net/wikiPrevBox/) (see "How to" on the project website) and other CMS
- Works in all modern browsers
- MIT license, open Source

## How-to
After the following step(s), all links to a Wikipedia article on your website will automatically display a preview box with the article summary that opens on mouseover or a fingertip.

### 1) Copy, paste & go!

``Add the following line of code to the bottom of your web page, that's all - nothing else is needed.``
```
<script src="https://su-pa.net/wikiPrevBox/wikiPreviewBox.min.js"></script>
```

### 2) Or alternatively, grab the code and host it yourself
``Copy the folder "wikiPrevBox" to the root of your website and insert the following line of code at the bottom of your web page. See the comments in the source files if you want to edit it. `` 
```
<script src="/wikiPrevBox/wikiPreviewBox.min.js"></script>
```
<br>

### **CUSTOMIZE** (optional)
### **Affects all preview boxes** 
are part of the ```<script ...>```-tag; currently you can set two parameters:
>data-wikipreview="noimages"\
data-wikipreview="width=*value*"

**Example:**
```
<script data-wikipreview="noimages,width=250" src="..."></script>
```
- `noimages`  
If this value is set, only the summary text are displayed and no images; this can help reduce traffic in places with poor network conditions; or select the images you like to display.
- `width=...`  
 Width of the preview boxes, number of pixels, value between 200 and 400, default is 300.  
 <br>
   
### **Affects a specific preview box** 
are part of a Wikipedia link; currently you can set two parameters:
>#nopreview\
#showimage

**Example:**
```
<a href="https://en.wikipedia.org/wiki/Lanyu#nopreview">Orchid Island</a>
```
- `#nopreview`  
Does not display the Wikipedia preview box at a specific link, but resets it to a normal link to a Wikipedia article.
- `#showimage`  
Set this, if you have used `noimages` in the `<script ...>` tag (see above) but still want to show a picture in a specific Wikipedia preview box.
<br><br> 

### **Changes via stylesheet**
You can overwrite the CSS rules of the preview boxes in your own stylesheet.
#### **Change the color of the Wikipedia links, e.g.**
`a.wikiLink {color: darkgreen;}`		      /* *link color* \*/\
`a:hover.wikiLink {color: orangered;}`  	/* *mouseover/fingertip* \*/\
`a:active.wikiLink {color: orangered;}` 	/* *mouse onclick/fingertip* \*/\

## About & privacy
Get the information on the [project page](https://su-pa.net/wikiPrevBox/) 

## Future plans, ideas
- Offline storing/cache requests locally to prevent doing same things twice (reduce electron travels:)
- Portrait modus on mobile: show image next to the summary text
- Custom text lenght of (a specific) preview box(es)
- ... 

## How to support?
- Become a "The Horse" member! It doesn't cost you a nickel! :-)\
 <a href="https://su-pa.net/wikiPrevBox/?the-horse" target="_blank"  rel="noopener">See what this means</a> (project website)
- <a href="https://donate.wikimedia.org/" target="_blank"  rel="noopener">Make a donation</a> to the 
				<a href="https://en.wikipedia.org/wiki/Wikimedia_Foundation" target="_blank" rel="noopener">Wikimedia Foundation</a>

## License
MIT License\
su-pa.net &copy; 11/2021