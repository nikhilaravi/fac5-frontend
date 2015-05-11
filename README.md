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
