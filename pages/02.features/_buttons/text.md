---
title: Buttons
styles: center-title
image_align: right
markdown:
    extra: true
---

### Use markdown extra for styled buttons

To add [*markdown extra*](http://learn.getgrav.org/content/headers#markdown) on a per page basis, add the following to your page header:

```prettyprint
markdown:
  extra: true
```
All button styles require an additional class to be added. This is done with markdown extra by appending the class in curly brackets directly after the markdown link code. Consecutive style classes should be separated with a space.

```prettyprint
[Title](link){.class .otherclass}
```
Use browser developer tools to see the styles of the buttons show here.

[Primary Color](#buttons){.button} [Secondary Color](#buttons){.button .secondary} [Success](#buttons){.success .button} [Alert](#buttons){.alert .button} [Warning](#buttons){.warning .button} [Disabled](#buttons){.disabled .button}

[Primary Color](#buttons){.button .hollow} [Secondary Color](#buttons){.button .secondary .hollow} [Success](#buttons){.success .button .hollow} [Alert](#buttons){.alert .button .hollow} [Warning](#buttons){.warning .button .hollow}

[Tiny](#buttons){.button .tiny} [Small](#buttons){.button .small} [Standard](#buttons){.button} [Large](#buttons){.button .large}  

[Expanded Button](#buttons){.button .expanded}