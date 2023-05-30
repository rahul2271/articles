# What is Media Query?

**Media queries** allow you to apply CSS styles depending on a device's general type (such as print vs. screen) or other characteristics such as screen resolution or browser viewport width. Media queries are used for the following:

* To conditionally apply styles with the CSS `@media` and `@import` at-rules.
    
* To target specific media for the `<style>`, `<link>`, `<source>`, and other HTML elements with the `media=` attribute.
    
* To test and monitor media states using the `Window.matchMedia()` and `MediaQueryList.addListener()` JavaScript methods.
    

## Syntax

A media query consists of a media type and can contain one or more expressions, which resolve to either be true or false.

> ### Example:
> 
> ```xml
> @media not|only mediatype and (expressions) {
>   CSS-Code;
> }
> ```

## Media Queries Simple Examples

One way to use media queries is to have an alternate CSS section right inside your style sheet.

The following example changes the background-color to light green if the viewport is 480 pixels wide or wider (if the viewport is less than 480 pixels, the background color will be pink ).

%[https://codepen.io/ZuberUstad/embed/OJwWoxE?default-tab=html%2Cresult] 

The following example shows a menu that will float to the left of the page if the viewport is 480 pixels wide or wider (if the viewport is less than 480 pixels, the menu will be on top of the content):

%[https://codepen.io/ZuberUstad/embed/mdjRGqX?default-tab=html%2Cresult] 

# Resources

### [w3school](https://www.w3schools.com/) [MDN](https://developer.mozilla.org/en-US/)