# fac5-frontend
Week 1 front end seminar


##Mobile First Design  
* We are designing our blog "Mobile first" - i.e. starting with mobile in mind and not the desktop browser  
* The advantages are... 
 * Desktop sites often have more functionality / fancy things than the equivalent mobile site; starting with the desktop means we have to remove things for the mobile, whereas starting with the mobile site we can add things for the desktop, which is simpler
 * Faster loading time on a mobile - otherwise the desktop version loads and components are removed which takes longer
 * Google page ranking higher for mobile optimized sites - easier to start with designing for mobile
 * Changing user habits - 25% of U.S. population only use mobiles for internet
 
More info [here](http://designshack.net/articles/css/mobilefirst/)

##HTML Validation 
* Checks the syntax of Web documnets written in formats such as HTML or XHTML
* Why? If you have errors in your code, different browers will interpret them in different ways
* Run your HTML documents through a Markup Validator such as the one run by W3C [here](https://validator.w3.org/)  

##CSS intro  

* As we probably all know by now, we use CSS to style our HTML  
 * Instead of writing out the colo(u)r/font/font-size for each HTML element inside the main HTML doc, we can have a separate CSS doc where we define how each HTML element should look  
 * Even better, we can use the class and ID attributes to specify (only) a single element (by ID) or multiple elements (by class)  
 * In the CSS, the class selector is the class name preceded by a full stop - .headers  
 * And the ID selector is the ID name preceded by a hashtag - #MainHeader  
 * TOP TIP - you can write links directly to a ID element - domain.com/page**#IDname** takes you directly to the IDname element on domain.com/page

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

## Web Accessibility  

* We want our content to be easily accessible - this could be to aid people with visual impairments, for example, but is also of general importance
 * When it comes down to it, only a human can really determine the accessibility of a web page, but [WAVE](http://wave.webaim.org/) or other tools can help identify errors automatically
  * For example, you might have some text on a background that comes up with poor contrast and is therefore hard to read - like so  
![Poor contrast example image](http://www.spaboomblog.com/wp-content/uploads/2007/08/low-contrast03.gif)
