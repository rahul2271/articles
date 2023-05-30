# What is Positioning in CSS?   
> The CSS position property is used to set position for an element. it is also used to place an element behind another and also useful for scripted animation effect.

# Property of Positioning 

>The position property specifies the type of positioning method used for an element. 
## Types of  Positioning :
>>- static
>>- relative
>>- fixed
>>- absolute
>>- sticky

> Elements are then positioned using the top, bottom, left, and right properties. However, these properties will not work unless the position property is set first. They also work differently depending on the position value.
### 1. position: static;
> This is a by default position for HTML elements. It always positions an element according to the normal flow of the page. It is not affected by the top, bottom, left and right properties.


<iframe height="300" style="width: 100%;" scrolling="no" title="posi" src="https://codepen.io/ZuberUstad/embed/wvxzOZY?default-tab=html%2Cresult" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/ZuberUstad/pen/wvxzOZY">
  posi</a> by Zuber Ustad (<a href="https://codepen.io/ZuberUstad">@ZuberUstad</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

### 2. position: fixed;
> An element with position: fixed; is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used to position the element.

<iframe height="300" style="width: 100%;" scrolling="no" title="relative pos" src="https://codepen.io/ZuberUstad/embed/abjmMgZ?default-tab=html%2Cresult" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/ZuberUstad/pen/abjmMgZ">
  relative pos</a> by Zuber Ustad (<a href="https://codepen.io/ZuberUstad">@ZuberUstad</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

### 3. position: relative;
> The relative positioning property is used to set the element relative to its normal position.

<iframe height="300" style="width: 100%;" scrolling="no" title="relative pos" src="https://codepen.io/ZuberUstad/embed/zYLKbgq?default-tab=html%2Cresult" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/ZuberUstad/pen/zYLKbgq">
  relative pos</a> by Zuber Ustad (<a href="https://codepen.io/ZuberUstad">@ZuberUstad</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>


### 4. position: absolute;
> The absolute positioning is used to position an element relative to the first parent element that has a position other than static. If no such element is found, the containing block is HTML.


<iframe height="300" style="width: 100%;" scrolling="no" title="absolute pos" src="https://codepen.io/ZuberUstad/embed/JjBRVPE?default-tab=html%2Cresult" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/ZuberUstad/pen/JjBRVPE">
  absolute pos</a> by Zuber Ustad (<a href="https://codepen.io/ZuberUstad">@ZuberUstad</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe> 
 
### 5. position: sticky;

> An element with *position: sticky;* is positioned based on the user's scroll position. <br>
> A sticky element toggles between *relative* and *fixed*, depending on the scroll position. It is positioned relative until a given offset position is met in the viewport - then it "sticks" in place (like position:fixed).

<iframe height="300" style="width: 100%;" scrolling="no" title="sticky pos" src="https://codepen.io/ZuberUstad/embed/bGjwJbO?default-tab=html%2Cresult" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/ZuberUstad/pen/bGjwJbO">
  sticky pos</a> by Zuber Ustad (<a href="https://codepen.io/ZuberUstad">@ZuberUstad</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>


<br>

# Resources 
[Javapoint](https://www.javatpoint.com/css-position) 
[W3school](https://www.w3schools.com/)
