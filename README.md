# CSS Grid


## Introduction
> CSS Grid layout, or simply Grid, is a two-dimensional grid-based layout system aims for the design of grid-based user interfaces. It is the very first CSS module created specifically to solve the layout problems; this module provides a series of properties designed specifically to create grids on screen. Grid layout works by applying CSS rules both to a parent element (which becomes the Grid Container) and to that elements children (which become Grid items).

## Terminology
* Grid Container - The element on which `display: grid` property is applied. It's the direct parent of all the grid items.
* Grid Item - Each child element placed in the grid container.

**Example:**
```html
<div class="container">
    <div class="Item 1">Child of container</div>
    <div class="Item 2">Child of container</div>
    <div class="Item 3">Child of container</div>
</div>
```
* Grid Line - The dividing lines that make up the structure of the grid.

![Grid Line](./img/grid-line.png)

* Grid Track - The space between two adjacent grid lines.

![Grid Track](./img/grid-track.png)

* Grid Cell - The space between two adjacent row grid lines and two adjacent column grid lines.

![Grid Cell](./img/grid-cell.png)

* Grid Area - A cell or multiple cells that mark the space in which a grid item will be placed.

![Grid Area](./img/grid-area.png)

![Grid Term](./img/Grid_term.odt)


> To get started you have to define a container element as a grid and applied `display: grid` property into it, set the column and row sizes with `grid-template-columns` and `grid-template-rows` properties, and then place its child elements into the grid with `grid-column` and `grid-row`.


## Parent Properties
* display - It defines the element as a grid container and establishes a new grid formatting context for its contents.
```display
    .container {
        display: value;
    }

    where value:
      * grid - generates a block-level grid
      * inline-grid - generates an inline-level grid
      * subgrid - if the grid container is a nested grid, this property indicates that the sizes of its rows / columns are to be taken from its parent.
```
      
