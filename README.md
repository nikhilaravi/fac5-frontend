# fac5-frontend
Week 1 front end seminar

##Contents

* [Mobile First Design](#mobile-first-design)
* [HTML Validation](#html-validation)
* [CSS Intro](#css-intro)
* [CSS Positioning](#css-positioning)
* [Web Accessibility](#web-accessibility)
* [Chrome Dev Tools](#chrome-dev-tools)




##Mobile First Design  
* We are designing our blog "Mobile first" - i.e. starting with mobile in mind and not the desktop browser  
* The advantages are... 
 * Desktop sites often have more functionality / fancy things than the equivalent mobile site; starting with the desktop means we have to remove things for the mobile, whereas starting with the mobile site we can add things for the desktop, which is simpler
 * Faster loading time on a mobile - otherwise the desktop version loads and components are removed which takes longer
 * Google page ranking higher for mobile optimized sites - greater exposure with designing for mobile
 * Changing user habits - 25% of U.S. population only use mobiles for internet
 
More info [here](http://designshack.net/articles/css/mobilefirst/)

##HTML Validation 
* Checks the syntax of Web documnets written in formats such as HTML or XHTML
* Why? If you have errors in your code, different browers will interpret them in different ways
* Run your HTML documents through a Markup Validator:
	* [W3C](https://validator.w3.org/)  

##CSS intro  

###Vanilla 

* We are encouraged to code without preprocessors,frameworks and templates.
* Don't rely on SASS & LESS.
* However, it is useful to be inspired by pre-existing code but we aim to have written all our code ourself to fully understand what's going on.

###IDs and Classes

* As we probably all know by now, we use CSS to style our HTML  
 * Instead of writing out the colo(u)r/font/font-size for each HTML element inside the main HTML doc, we can have a separate CSS doc where we define how each HTML element should look  
 * Even better, we can use the class and ID attributes to specify (only) a single element (by ID) or multiple elements (by class)  
 * In the CSS, the class selector is the class name preceded by a full stop - .headers  
 * And the ID selector is the ID name preceded by a hashtag - #MainHeader  

###Media Queries

 * We can also specify different rules for different screen sizes, device types, page orientations etc. using CSS Media Queries  
  * So we can make images bigger on larger screens, or remove menus/headers for print-friendly pages, and so on  
 
 
```css
//Normal CSS 
#main-header {
	font-family: arial;
	color: purple;
}


//Change font and color when orientation is portrait (not that you would want to...)

@media (orientation: portrait) {
	#main-header {
		font-family: Times;
		color: green;
	}
}
```
* Test your device to see which queries satisfied with this [link](http://cssmediaqueries.com/overview.html).
  * Note handheld does not refer to iphones etc. but very old dated phones!
* More useful links [here](https://developers.google.com/web/fundamentals/layouts/rwd-fundamentals/use-media-queries?hl=en) and [here](http://www.w3schools.com/cssref/css3_pr_mediaquery.asp)

##CSS Positioning

There are four types of positioning you can apply to your elements.
* Static
 * The default value. Elements with static position will be positioned in their natural place in the page. Usually the top left of the page.
* Relative
 * Relative elements behave the same as static elements, but can be manually positioned using the 'top', 'right', 'left' and 'bottom' properties.
* Fixed
 * Fixed elements are positioned relative to the viewport ('top', 'left' etc...), but will always stay in the same place on the screen, even as the page is scrolled.
* Absolute
 * Absolutely positioned elements are dependent on their parent. If they are inside a positioned element (anything except static), they are positioned relative to that container, else they are positioned relative to the viewport.

###Float
* Float can be used to wrap text around images. Images can be floated left or right.
* Other elements in the same container need to be cleared so they don't overlap the floated elements.

## Web Accessibility  

* We want our content to be easily accessible - this could be to aid people with visual impairments, for example, but is also of general importance
 * When it comes down to it, only a human can really determine the accessibility of a web page, but [WAVE](http://wave.webaim.org/) or other tools can help identify errors automatically
  * For example, you might have some text on a background that comes up with poor contrast and is therefore hard to read - like so  
![Poor contrast example image](http://www.spaboomblog.com/wp-content/uploads/2007/08/low-contrast03.gif)

##Chrome Dev Tools
Interactive tool to live edit and test and HTML/CSS on existing websites
To open dev tools click on **View > Developer Tools**

Some cool things you can do:
* View the mobile version of a site - click the little mobile phone icon in the top left of the developer tools window
* Inspect element- view the HTML/CSS associated with elements on the web page. Click on the little magnifying glass in the dev tools window and move it across the webpage, hovering over the elements you want to investigate. If you click, it will take you to the relevant section in the code
* Live edit HTML and CSS - change HTML/CSS properties in the dev tools window and see the website change in response! To increment numerical CSS values, use the up and down arrows. A strikethrough on the CSS value shows that the property value has been overridden- e.g in a list the individual ``` <li> ``` list element has inherited a color value from its parent ``` <ul> ``` class, but this may be replaced if a different colour is specified for ``` <li> ``` elements. 
* Test different layouts-move around sections of the HTML by dragging and dropping
* View the box model- scroll down on the right hand side of the dev tools window and you'll see a set of rectangles - this shows the dimensions of the content, padding and the border. 



Lots more info [here](https://developer.chrome.com/devtools/docs/dom-and-styles) on the Dev Tools website.
>>>>>>> 8662dcd926d7a014f3d64d208cf7d4994d552d04
