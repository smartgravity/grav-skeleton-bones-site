---
title: 'Columns with Markdown'
summary:
    enabled: '1'
    format: short
taxonomy:
    tag:
        - Columns
    category:
        - documentation
content:
    limit: 5
    pagination: '1'
    order:
        dir: desc
        by: date
    items: '@self.children'
---

**You can choose how many columns** and our twig template calculates the column numbers for smaller screens for you! We're using a couple cool things to make this happen:

- [Grav's markdown divider trick](http://learn.getgrav.org/cookbook/general-recipes#render-content-in-columns)
- [Foundation's Block Grid classes](http://foundation.zurb.com/sites/docs/grid.html#block-grids)
- [Twig's Math functions](http://twig.sensiolabs.org/doc/templates.html#math)

This is a **modular** template so you can find it in the theme's `/templates/partials/modular/' directory with the name **columns.html.twig**. There is even a dropdown option in the Admin Plugin so you can easily choose how many columns you'd like to use!

If not using the Admin Plugin, you can add the following to the page header to set the number of columns to be used:

```prettyprint
column_number: '3'
```
>>> Remember the options are 2,3,4,5,6,7,8 only!

With this being a grid based on "12", we have options from 2 columns to 8 columns. If you're an advanced developer or looking for a project, Foundation has a variable for [changing the number of columns](http://foundation.zurb.com/sites/docs/grid.html#multiple-grids) the grid is based on, so this is all customizable for those far reaching project requirements.

The columns have a `<div class="sg-column-block">` added to them in the template. There are corresponding color styles that you can add to your column blocks and you add them to your page header...or just through the Admin Plugin interface.

For your content, each column block is divided with three dashes `---`.

```prettyprint
### First Block

This is the first column in the set

---
### Second Block

This is the second column in the set

---

### Third Block

This is the third column in the set
```
