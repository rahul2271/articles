# FlexBox
>Flex box aims at providing a more efficient way to lay out, align and distribute space among items in a container, even when their size is unknown and/or dynamic  

<br>

# FlexBox Layout 

> FlexBox is not a single Property its a whole module, it contains a lot of things including its whole set of properties. <br>
Some of them are meant to be set on the container parent element, known as **flex container** whereas the others are meant to be set on the children said **flex items**.

## Layout 
![FlexBox layout](https://css-tricks.com/wp-content/uploads/2018/11/00-basic-terminology.svg)

> In this layout items will be laid out either the *main-axix*(from main-start to main -end ) or the *cross-axis*(cross-start to cross-end).

>> - **main axis** – The main axis of a flex container is the primary axis along which flex items are laid out. Beware, it is not necessarily horizontal,it depends on the *flex-direction property* .

>> - **main-start | main-end** – The flex items are placed within the container starting from main-start and going to main-end.

>> - **main size** – A flex item’s width or height, whichever is in the main dimension, is the item’s main size. The flex item’s main size property is either the ‘width’ or ‘height’ property, whichever is in the main dimension.


>>- **cross axis** – The axis perpendicular to the main axis is called the cross axis. Its direction depends on the main axis direction.


>> - **cross-start | cross-end** – Flex lines are filled with items and placed into the container starting on the cross-start side of the flex container and going toward the cross-end side.

>> - **cross size** – The width or height of a flex item, whichever is in the cross dimension, is the item’s cross size. The cross size property is whichever of ‘width’ or ‘height’ that is in the cross dimension.

# FlexBox Property 

## Container and Items
>Below is the example of Container and Items
>> In this example the box is called *Container* and inside the  container is called *items*

>>In FlexBox Container are also know as *parent* or* flex-container*

>> Same for items its known *child* or *flex-items*


<iframe height="300" style="width: 100%;" scrolling="no" title="Items and container" src="https://codepen.io/ZuberUstad/embed/eYjdvEg?default-tab=html%2Cresult" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/ZuberUstad/pen/eYjdvEg">
  Items and container</a> by Zuber Ustad (<a href="https://codepen.io/ZuberUstad">@ZuberUstad</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

## Properties for the Parent  or Flex Container

## Display 
>> Display Defines a flex-container either will be in inline or block depending on the user.By default its a block 

    .container{
        display:flex; /* or inline-flex*/
    }

## Flex-direction 
>> It establishes the main-axis and defining the direction of flex items are placed in the flex container. Flexbox is  a single-direction layout concept. Think of flex items as primarily laying out either in horizontal rows or vertical columns.

```
    *container{
          flex-direction: row | row-reverse | column | column-reverse;
    }
```
## Example : 

<iframe height="300" style="width: 100%;" scrolling="no" title="Items and container" src="https://codepen.io/ZuberUstad/embed/rNrMyzy?default-tab=html%2Cresult" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/ZuberUstad/pen/rNrMyzy">
  Items and container</a> by Zuber Ustad (<a href="https://codepen.io/ZuberUstad">@ZuberUstad</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>


## Flex-Wrap

>>By default, flex items will all try to fit onto one line. You can change that and allow the items to wrap as needed with this property.


```
.container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}

```

## justify-content
>> It defines the alignment along the main axis. It helps distribute extra free space leftover when either all the flex items on a line are inflexible, or are flexible but have reached their maximum size. It also exerts some control over the alignment of items when they overflow the line.


```
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;
}

```


<iframe height="300" style="width: 100%;" scrolling="no" title="justify-content" src="https://codepen.io/ZuberUstad/embed/gOjwWWP?default-tab=html%2Cresult" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/ZuberUstad/pen/gOjwWWP">
  justify-content</a> by Zuber Ustad (<a href="https://codepen.io/ZuberUstad">@ZuberUstad</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

## align-items
>>This defines the default behavior for how flex items are laid out along the cross axis on the current line. Think of it as the justify-content version for the cross-axis (perpendicular to the main-axis).  

```
.container {
  align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end + ... safe | unsafe;
}

```

<iframe height="300" style="width: 100%;" scrolling="no" title="align-items" src="https://codepen.io/ZuberUstad/embed/oNMzWWR?default-tab=html%2Cresult" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/ZuberUstad/pen/oNMzWWR">
  align-items</a> by Zuber Ustad (<a href="https://codepen.io/ZuberUstad">@ZuberUstad</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>
</iframe>



# Properties for the Children i.e flex items

## order
>>By default, flex items are laid out in the source order. However, the order property controls the order in which they appear in the flex container.

```
.item {
      order: 5; /* default is 0 */
}

```


<iframe height="300" style="width: 100%;" scrolling="no" title="order" src="https://codepen.io/ZuberUstad/embed/QWBKvOM?default-tab=html%2Cresult" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/ZuberUstad/pen/QWBKvOM">
  order</a> by Zuber Ustad (<a href="https://codepen.io/ZuberUstad">@ZuberUstad</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>


## flex-shrink
>> This defines the ability for a flex item to shrink if necessary.

``` 
.item {
         flex-shrink: 3; /* default 1 */
}
```


## Flex-basis
>>This defines the default size of an element before the remaining space is distributed. It can be a length (e.g. 20%, 5rem, etc.) or a keyword.


```
.item {
  flex-basis:  | auto; /* default auto */
}

```

## flex
>> This is the shorthand for flex-grow, flex-shrink and flex-basis combined. The second and third parameters (flex-shrink and flex-basis) are optional. The default is 0 1 auto, but if you set it with a single number value, like flex: 5;, that changes the flex-basis to 0%, so it’s like setting flex-grow: 5; flex-shrink: 1; flex-basis: 0%;.

```
.item {
  flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
}
```


## align-self
>> This allows the default alignment (or the one specified by align-items) to be overridden for individual flex items.


```
.item {
  align-self: auto | flex-start | flex-end | center | baseline | stretch;
}
```

# Resources 
[FlexBox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
[W3school](https://www.w3schools.com/)



