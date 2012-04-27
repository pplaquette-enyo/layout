This is a layout library for Enyo 2. This library provides a collection of layout functionality

The list package provides a `List` control that displays a scrolling list of rows. It's suitable for displaying very large lists and is optimized such that only a small portion of the list is rendered
at a given time. 

Check out the [List sample](http://enyojs.com/samples/list/list-contacts.html) to see it in action.

The fittable pacakge helps you create layouts that expand to fit available space -- a common need for apps, but one that has historically been difficult to meet using web technologies.

The  `FittableColumns` and `FittableRows` controls let you define views whose children are arranged either horizontally or vertically. Within a given view, you can designate one child to expand and contract to fit the available space, while its siblings retain their natural or explicitly specified sizes. Fittable views can be nested as needed.

If you're thinking that this sounds a lot like a limited version of the CSS Flexible Box Model, you're right. Our main objective was to provide a layout model with capabilities similar to Flex Box, but with greater browser compatibility. We also wanted to impose as few limitations as possible on the CSS styling of child components, and to use JavaScript sparingly (we use it to calculate the height of fittable elements, but otherwise leave the layout work to the browser).

As much as we like them, we want to emphasize that you should only use `FittableColumns` and `FittableRows` when you need views to expand and contract to fit available space. If you simply want to arrange elements horizontally or vertically, you're better off employing standard web layout techniques.

Check out the [Fittable sample](http://enyojs.com/samples/fittable/app-layouts.html) to see `FittableColumns` and `FittableRows` in action.