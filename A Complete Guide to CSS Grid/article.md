# What is CSS Grid

> CSS Grid Layout (aka “Grid” or “CSS Grid”), is a two-dimensional grid-based layout system that, compared to any web layout system of the past, completely changes the way we design user interfaces.
> 
> CSS has always been used to lay out our web pages, but it’s never done a very good job of it.
> 
> First, we used tables, then floats, positioning and inline-block, but all of these methods were essentially hacks and left out a lot of important functionality (vertical centering, for instance).
> 
> Flexbox is also a very great layout tool, but its one-directional flow has different use cases — and they actually work together quite well! Grid is the very first CSS module created specifically to solve the layout problems we’ve all been hacking our way around for as long as we’ve been making websites.

# Important CSS Grid terminology

Before diving into the concepts of Grid it’s important to understand the terminology.

Following are the terms in CSS Grid

1. Grid Container
    
2. Grid Items
    
3. Grid Line
    
4. Grid Cell
    
5. Grid Track
    
6. Grid Area
    

## Grid Container

> The element on which the display: grid is applied. It’s the direct parent of all the grid items. In this example container is the grid container.

```xml
<div class="container">
  <div class="item item-1"> </div>
  <div class="item item-2"> </div>
  <div class="item item-3"> </div>
</div>
```

## Grid Items

> The children (i.e. direct descendants) of the grid container. Here the item elements are grid items, but the sub-item isn’t.

```xml
<div class="container">
  <div class="item"> </div>
  <div class="item">
    <p class="sub-item"> </p>
  </div>
  <div class="item"> </div>
</div>
```

## Grid Line

> The dividing lines make up the structure of the grid. They can be either vertical (“column grid lines”) or horizontal (“row grid lines”) and reside on either side of a row or column. Here the yellow line is an example of a column grid line.

![Grid line](https://css-tricks.com/wp-content/uploads/2018/11/terms-grid-line.svg align="left")

## Grid Cell

> The space between two adjacent rows and two adjacent column grid lines. It’s a single “unit” of the grid. Here are the grid cell between row grid lines 1 and 2, and column grid lines 2 and 3.

![Grid Cell](https://css-tricks.com/wp-content/uploads/2018/11/terms-grid-cell.svg align="left")

## Grid Track

> The space between two adjacent grid lines. You can think of them as the columns or rows of the grid. Here’s the grid track between the second and third-row grid lines.

![Grid tack](https://css-tricks.com/wp-content/uploads/2021/08/terms-grid-track.svg align="left")

## Grid Area

> The total space surrounded by four grid lines. A grid area may be composed of any number of grid cells. Here’s the grid area between row grid lines 1 and 3, and column grid lines 1 and 3.

![Grid area](https://css-tricks.com/wp-content/uploads/2018/11/terms-grid-area.svg align="left")

# CSS Grid properties

## Properties for the Parent (Grid Container)

* display
    
* grid-template-columns
    
* grid-template-rows
    
* grid-template-areas
    
* grid-template
    
* grid-column-gap
    
* grid-row-gap
    
* grid-gap
    
* justify-items
    
* align-items
    
* place-items
    
* justify-content
    
* align-content
    
* place-content
    
* grid-auto-columns
    
* grid-auto-rows
    
* grid-auto-flow
    
* grid
    

### Display

Defines the element as a grid container and establishes a new grid formatting context for its contents.

Values:

- grid – generates a block-level grid 
-   inline-grid – generates an inline-level grid

```xml
.container {
  display: grid | inline-grid;
}
```

### Grid-template-columns & Grid-template-rows

Defines the columns and rows of the grid with a space-separated list of values. The values represent the track size, and the space between them represents the grid line.

Values:

* `<track-size>` – can be a length, a percentage, or a fraction of the free space in the grid using the fr unit (more on this unit over at DigitalOcean)
    
* `line-name>` – an arbitrary name of your choosing
    

```xml
.container {
  grid-template-columns: ...  ...;
  /* e.g. 
      1fr 1fr
      minmax(10px, 1fr) 3fr
      repeat(5, 1fr)
      50px auto 100px 1fr
  */
  grid-template-rows: ... ...;
  /* e.g. 
      min-content 1fr min-content
      100px 1fr max-content
  */
}
```

## gap

A shorthand for row-gap and column-gap Values:

* `<grid-row-gap> <grid-column-gap>` – length values
    

```xml
.container {
  /* standard */
  gap: <grid-row-gap> <grid-column-gap>;

  /* old */
  grid-gap: <grid-row-gap> <grid-column-gap>;
}
```

## justify-items

Aligns grid items along the inline (row) axis (as opposed to align-items which aligns along the block (column) axis). This value applies to all grid items inside the container.

Values:

* start – aligns items to be flush with the start edge of their cell
    
* end – aligns items to be flush with the end edge of their cell
    
* center – aligns items in the center of their cell
    
* stretch – fills the whole width of the cell (this is the default)
    

```xml
.container {
  justify-items: start | end | center | stretch;
}
```

## align-items

Aligns grid items along the block (column) axis (as opposed to justify-items which aligns along the inline (row) axis). This value applies to all grid items inside the container.

Values:

* stretch – fills the whole height of the cell (this is the default)
    
* start – aligns items to be flush with the start edge of their cell
    
* end – aligns items to be flush with the end edge of their cell
    
* center – aligns items in the center of their cell
    
* baseline – align items along text baseline. There are modifiers to baseline — first baseline and last baseline which will use the baseline from the first or last line in the case of multi-line text.
    

```xml
.container {
  align-items: start | end | center | stretch;
}
```

## Properties for the Children (Grid Items)

* grid-column-start
    
* grid-column-end
    
* grid-row-start
    
* grid-row-end
    
* grid-column
    
* grid-row
    
* grid-area
    
* justify-self
    
* align-self
    
* place-self
    

### grid-column-start , grid-column-end ,grid-row-start ,grid-row-end

Determines a grid item’s location within the grid by referring to specific grid lines. grid-column-start/grid-row-start is the line where the item begins, and grid-column-end/grid-row-end is the line where the item ends.

Values:

* `<line>` – can be a number to refer to a numbered grid line, or a name to refer to a named grid line
    
* `span <number>` – the item will span across the provided number of grid tracks
    
* `span <name>` – the item will span across until it hits the next line with the provided name
    
* `auto` – indicates auto-placement, an automatic span, or a default span of one
    

```xml
.item {
  grid-column-start: <number> | <name> | span <number> | span <name> | auto;
  grid-column-end: <number> | <name> | span <number> | span <name> | auto;
  grid-row-start: <number> | <name> | span <number> | span <name> | auto;
  grid-row-end: <number> | <name> | span <number> | span <name> | auto;
}
```

### justify-self

Aligns a grid item inside a cell along the inline (row) axis (as opposed to align-self which aligns along the block (column) axis). This value applies to a grid item inside a single cell.

Values:

* start – aligns the grid item to be flush with the start edge of the cell
    
* end – aligns the grid item to be flush with the end edge of the cell
    
* center – aligns the grid item in the center of the cell
    
* stretch – fills the whole width of the cell (this is the default)
    

```xml
.item {
  justify-self: start | end | center | stretch;
}
```

### align-self

Aligns a grid item inside a cell along the block (column) axis (as opposed to justify-self which aligns along the inline (row) axis). This value applies to the content inside a single grid item.

Values:

* start – aligns the grid item to be flush with the start edge of the cell
    
* end – aligns the grid item to be flush with the end edge of the cell
    
* center – aligns the grid item in the center of the cell
    
* stretch – fills the whole height of the cell (this is the default)
    

```xml
.item {
  align-self: start | end | center | stretch;
}
```

# Resources

[css-tricks](https://css-tricks.com/snippets/css/complete-guide-grid/)