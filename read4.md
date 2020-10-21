# css GRID

* The `grid-column-start` property defines on which column-line the item will start.

* a span, or nothing (automatic) to its grid placement. This start position defines the block-start edge of the grid area.
  * `grid-column-start: span 3;`

## Properties for the Parent

* display
  * `.container {display: grid | inline-grid;}`

* grid-template-rows /columns
  * `.container {`</br>
`  grid-template-columns:  40px 50px auto 50px 40px;`</br>
 ` grid-template-rows:  25% 100px auto;}`
 
 ![](https://css-tricks.com/wp-content/uploads/2018/11/template-columns-rows-01.svg)

* grid-template-areas
  * `.container {`</br>
    `"header header header header"`</br>
    `"main main . sidebar"`</br>
    `"footer footer footer footer";}`

    ![areas](https://css-tricks.com/wp-content/uploads/2018/11/dddgrid-template-areas.svg)

* grid-template
  * `.container {`</br>
    `grid-template: none | <grid-template-rows> /  <grid-template-columns>;}`

* row/column-gap
  * ` .container { `</br>
    `grid-template-columns: 100px 50px 100px;`</br>
    `grid-template-rows: 80px auto 80px;`</br>
    `column-gap: 10px;`</br>
    `row-gap: 15px; }`
  ![](https://css-tricks.com/wp-content/uploads/2018/11/dddgrid-gap.svg)


## Properties for the Children

* grid start/end
  * `.item-a {`
    `grid-column-start: 2;`
    `grid-column-end: five;`
    `grid-row-start: row1-start;`
    `grid-row-end: 3;}`

![](https://css-tricks.com/wp-content/uploads/2018/11/grid-column-row-start-end-01.svg)

* grid-row/column
  * `.item-c {`
    `grid-column: 3 / span 2;`
    `grid-row: third-line / 4;}`

![](https://css-tricks.com/wp-content/uploads/2018/11/grid-column-row.svg)

* grid-area
  * `.item-d {  grid-area: header;}`

![](https://css-tricks.com/wp-content/uploads/2018/11/grid-area.svg)

* justify-self
  * `.item {  justify-self: start | end | center | stretch;}`
![](https://css-tricks.com/wp-content/uploads/2018/11/justify-self-center.svg)

* align-self
  * `.item {  align-self: start | end | center | stretch;}`
![](https://css-tricks.com/wp-content/uploads/2018/11/align-self-stretch.svg)

* place-self
  * `.item-a {  place-self: center;}`
![](https://css-tricks.com/wp-content/uploads/2018/11/place-self-center.svg)

