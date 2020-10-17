[BACK](https://abdullahmou.github.io/reading-notes/)
# Responsive Web Design

* With the growth in mobile Internet usage comes the question of how to build websites suitable for all users. The industry response to this question has become responsive web design, also known as RWD.
![](https://hackernoon.com/images/1tjg32bo.jpg)
</br>

## Responsive vs Adaptive vs Mobile

* Responsive and adaptive web design are closely related
![any](https://www.ibexa.co/var/site/storage/images/_aliases/ibexa_content_full/1/1/0/6/36011-4-eng-GB/IMPORT_jxVS4vadaptive-vs-responsive.png)
</br>

* Mobile, on the other hand, generally means to build a separate website commonly on a new domain solely for mobile users. While this does occasionally have its place, it normally isn’t a great idea.

* Currently the most popular technique lies within responsive web design,
![any](https://i2.wp.com/www.thinksys.com/wp-content/uploads/2017/04/responsiveDesign-blog.jpg?fit=700%2C400&ssl=1)
</br>

## Responsive Web Design is

* broken down into three main components, including
  * flexible layouts
  * media queries
  * flexible media

</br>

### Flexible Layouts

* is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.

* Flexible grids are built using relative length units, most commonly percentages or em units.

* These relative lengths are then used to declare common grid property values such as width, margin, or padding.

### Media Queries

* Initializing Media Queries

  * importing a new style sheet using the @import rule
  * linking to a separate style sheet from within the HTML document

* Logical Operators in Media Queries

  * help build powerful expressions. There are three different logical operators available for use within media queries, including (and), (not), and (only).

* Media Queries Demo

  * Using media queries we will now rewrite the flexible layout we built previously. One of the current problems within the demo appears when the aside width becomes uselessly small within smaller viewports.
  ![any](https://miro.medium.com/max/3060/1*M6fLqM8R9YTf8t2j-ahvRQ.png)
</br>

### Flexible Media

* The final, equally important aspect to responsive web design involves flexible media. As viewports begin to change size media doesn’t always follow suit. Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.
![any](https://i1.wp.com/css-tricks.com/wp-content/uploads/2012/09/flexible-images.jpg)
</br>
