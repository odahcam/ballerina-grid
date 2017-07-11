# ballerina-grid
Custom CSS responsive table-like grid system.

### Why ballerina?

It's flexible, beautifull and do things that almost no one can do.

## Getting started

You will need an structure that remembers a table, but it's more grid friendly than usual tables.

### Install

You can download the source directly from here and link the CSS files.

**OR**

You can install it via NPM and link the CSS files anyway. :p

By NPM you can control the version of the `ballerina-grid` you are using and also can easly update the package when updates are released!

```
npm install ballerina-grid --save
```

### Setting your HTML

#### The container

First of all, will you create a container: `<div class="ballerina">`.

That container supports some optional classes:

- `ballerina-<size>`: responsive classes in which `<sizes>` are breakpoints for turning the ballerina into a flexible table-like or a simple block element.
- `ballerina-align-<alignment>`: this will vertically align your columns inside a `.ballerina-row` (see next step).
- `ballerina-force`: never lets `.ballerina` be turned into a block element.

#### The row

Inside your container you can have as many rows as you want: `<div class="ballerina-row">`. Inside your rows you will put your columns.

```html
<div class="ballerina">

    <div class="ballerina-row">...</div>

    <div class="ballerina-row">...</div>

    <div class="ballerina-row">...</div>

    ...
    
</div>
```

#### The column

Finally the column element is: `<div class="ballerina-col">`.

Columns can have any child you want and **more**, columns can have a `<div class="ballerina">` inside it.

So your final structure will be something like:

```html

<div class="ballerina">


    <div class="ballerina-row">
    
        <div class="ballerina-col">...</div>
    
        <div class="ballerina-col">...</div>
    
    </div><!-- /.ballerina-row -->
    

    <div class="ballerina-row">
    
        <div class="ballerina-col">...</div>
    
        <div class="ballerina-col">...</div>
    
        <div class="ballerina-col">...</div>
        
    </div><!-- /.ballerina-row -->
    

    <div class="ballerina-row">
    
        <div class="ballerina-col">
        
        
            <div class="ballerina">
            

                <div class="ballerina-row">

                    <div class="ballerina-col">...</div>
                    
                </div><!-- /.ballerina-row -->
                
                
            </div><!-- /.ballerina -->
            
            
        </div><!-- /.ballerina-col -->
            
        <div class="ballerina-col">...</div><!-- /.ballerina-col -->
        
    </div><!-- /.ballerina-row -->
    

    ...
    
    
</div><!-- /.ballerina -->
```
