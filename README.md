# :dog: [Pug Snippets](https://github.com/nmsmith22389/Pug-Snippets) *(1.0.0)*

####Pug Snippets for Sublime Text
*Pug was formerly known as Jade*

## Installation
Install through [Package Control]() by pressing <kbd>⌘</kbd>+<kbd>SHIFT</kbd>+<kbd>P</kbd> (or <kbd>CTRL</kbd>+<kbd>SHIFT</kbd>+<kbd>P</kbd> for windows) and typing Pug Snippets

## Snippets

### Jade

#### Case

case =>
```pug
case variable
    when condition
        //- code
    default
        //- code
```

#### Conditionals

if =>  
```pug
if condition
    //- code
```

ife => 
```pug
if condition
    //- code
else
    //- code
```

unl =>
```pug
unless condition
    //- code
```

#### Doctype

doc =>
```pug
doctype html
```

docx =>
```pug
doctype xml
```

#### Filters

cof =>
```pug
:coffeescript
    # code
```

less =>
```pug
:less
    // code
```

md =>
```pug
:markdown
    <!-- code -->
```

styl =>
```pug
:stylus
    // code
```

#### Includes

inc =>
```pug
include file.pug
```

#### Inheritance

ext =>
```pug
extends file.pug
```

blk =>
```pug
block name
```

app =>
```pug
append name
```

pre =>
```pug
prepend name
```
*(according to the [docs](https://pugjs.org/language/inheritance.html#block-append-prepend), append and prepend do not need the `block` before them)*

#### Iteration

each =>  
```pug
each value in variable
    //- code
```

while =>  
```pug
while condition
    //- code
```

#### Mixins

mix =>
```pug
mixin name(param)
    //- code
```

#### Tags

a =>
```pug
a(href='http://') text
```

btn =>
```pug
button(type='submit') name
```

form =>
```pug
form(method='', action='')
```

img =>
```pug
img(src='path}', alt='')
```

inp =>
```pug
input(type='text')
```

link =>
```pug
link(rel='stylesheet', type='text/css', href='css/app.css')
```

script =>
```pug
script(src='js/app.js', type='application/javascript')
```

#### Attributes

aria =>
```pug
aria-=''
```

ariah =>
```pug
aria-hidden=true
```

class =>
```pug
class=''
```
*(this is supplied but I recommend using ex:`input(type='text').class` instead)*

data =>
```pug
data-=''
```

id =>
```pug
id=''
```
*(this is supplied but I recommend using ex:`input(type='text')#id` instead)*

#### CDNs

[FontAwesome](http://fontawesome.io/): fa =>
```pug
link(href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css", rel="stylesheet", integrity="sha384-wvfXpqpZZVQGK6TAh5PVlGOfQNHSoD2xbE+QkPxCAFlNEevoEH3Sl0sibVcOQVnN", crossorigin="anonymous")
```

[jQuery](https://jquery.com/): jq =>
```pug
script(src='https://code.jquery.com/jquery-3.1.1.min.js', integrity='sha256-hVVnYaiADRTO2PzUGmuLJr8BLUSjGIZsDYGmIJLv2b8=', crossorigin='anonymous')
```

#### Templates

html =>
```pug
doctype html
html
    head(lang='en')
        title title name
        meta(charset='UTF-8')
body
    Hello World!
```
