#Common Mistakes 
- do not understand css + html structure (modulization)
- using Id for css formating (not best practises)
- using inline coding for formate elements. (inline coding only be use for js/jquery perpose)
- do not use !important
- add class every div element
- do not use exatra elements
- when less/sass used do not add css in css file. always use less/sass for adding css

#What is css ?
- CSS, or Cascading Style Sheets, is a presentation ,  language created to style the appearance of content using, for example, fonts or colors.


## Type of stylesheet
    - In a separate file (external)

            <link rel="stylesheet" type="text/css" href="mystyle.css">
            
    - At the top of a web page document (internal)
    
            <style>
            body {
                background-color: linen;
            }
            
            h1 {
                color: maroon;
                margin-left: 40px;
            } 
            </style>

    - Right next to the text it decorates (inline)
    
            <h1 style="color:blue;margin-left:30px;">This is a heading.</h1>


# css concepts
- ## selector type
    - Id selector #myId
    - class selector .myClass
    - attr selector (a[alt="my image"])
    - http://www.w3schools.com/cssref/css_selectors.asp
- ## Inharit css properties
        .body{
            font-size:15px;
        }
    This will apply to all elements

- ## !important

        p.note
        1 class + 1 element = 11
        #sidebar p[lang="en"]
        1 ID + 1 attribute + 1 element = 111
        body #main .post ul li:last-child
        1 ID + 1 class + 1 pseudo-class + 3 elements = 123

- ## Box Modeling
    http://www.w3schools.com/css/css_boxmodel.asp
- ## Dispaly
- ## Floting Item vs aling item
- ## position (relative, absolute, fixed)
- ## inline , inline-block, block
- ## overflow
- ## combinators 'space' , > , + ~
- ## shorthand
        .box{
            background: #ffffff url("img_tree.png") no-repeat right top;
             padding:10px 15px 20px 30px;
        }
- ## Pseudo-classes selector
        /* unvisited link */
        a:link {
            color: #FF0000;
        }
        
        /* visited link */
        a:visited {
            color: #00FF00;
        }
        
        /* mouse over link */
        a:hover {
            color: #FF00FF;
        }
        
        /* selected link */
        a:active {
            color: #0000FF;
        }
- ## hiding element
    - by opacity:0
    - by display:none
    - by visibility:hidden
#Structure of css

## all css in one styles.css file.
- this is used for small project. 


##modulization and Component base css
- Bootstrap is the best example of component base css.
- [components](http://designmodo.github.io/Flat-UI/) 
http://designmodo.github.io/Flat-UI/

### for Big project css should be divided into
    - Base css
    - Layout css
    - Module css
    - State css
    - Theme css

#### example 
## base css
    html, body, form { margin: 0; padding: 0; }
    input[type=text] { border: 1px solid #999; }
    a { color: #039; }
    a:hover { color: #03C; }
    
## Layout css    
    .article {
        width: 80%;
        float: left;
    }
    
    .sidebar {
        width: 20%;
        float: right;
    }

## Module css
    html
        <div class="ProductRating">
          <img alt="Company logo" class="img-logo">
          <h3 class="ProductRating-title">Title</h3>
          <div class="u-starHolder">
            <span class="ProductRating-star ProductRating-star--active"></span>
            <span class="ProductRating-star ProductRating-star--active"></span>
            <span class="ProductRating-star ProductRating-star--active"></span>
            <span class="ProductRating-star"></span>
          </div>
        </div>
----------------------------   
        
css

    .ProductRating {
          ...
        }
        // nested element
        .ProductRating-title {
          ...
        }
        // nested element
        .ProductRating-star {
          ...
        }
        // nested element's modifier
        .ProductRating-star--active {
          ...
        }




# Important Link
## https://www.smashingmagazine.com/mastering-css-principles-comprehensive-reference-guide/
## http://www.w3schools.com/css/default.asp


Video 

https://www.youtube.com/watch?v=-65YXXhJvOE&list=PL0b6OzIxLPbw5xyi8Q6cdR05Gz-0x-vaf&index=1







