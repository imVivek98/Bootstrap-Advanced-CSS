TinDog Starting Files


The Box Model of CSS :

    Content - The content of the box, where text and images appear
    Padding - Clears an area around the content. The padding is transparent. i.e It is the area between the border and the content.
    Border - A border that goes around the padding and content.
    Margin - Clears an area outside the border. The margin is transparent. i.e. We can set the space between different box element by setting the margin.

    To set the space between different content items in the same box , we use padding.
---------------------------------------------------------------------------------------------------------------------------

Media Queries:

If we want our html elements to display different behaviour under different conditions , we use media queries.This is a native CSS feature that helps us to make our websites responsive without the use of bootstrap grids.

Eg : <h1>My name is Vivek</h1>

CSS:

h1{
  color:blue;
}

Eg:

@media print{  (print is the type.)
  h1{
    color:red;
  }
}

Here , the h1 element becomes red when it is about to be printed.
Other Keywords include screen (specifies screen size) , speech(becomes activated if the website is being read out for a visually impaired person) etc

The structure of a media query is as follows :
@media <type><feature>


Eg:
h1{
  font-size: 30px;
}

@media (max-width: 900px){ //Means less than or equal to 900px
  h1{
    font-size: 100px;
  }
}

We can also use multiple conditions:

Eg:

@media (min-width:500px) and (max-width:700px){  //Action will execute in the 200px between 500 and 700px.
  //////Action/////
}


- View port means the size of the screen on which the the website is rendered.

-------------------------------------------------------------------------------------------------------------------------

  ID's > Classes > html elements --> This is the hierarchy of elements while styling.So , ID's have the highest ranking and if you have a different attribute in classes and different in a particular ID , then ID attribute is what gets enforced.


Combining Selectors:

1. selector1 , selector2{

}

Eg: h1 , p{
  color:red;
}

2. Hierarchical selectors :

parent child{

}

Eg: div .title{   // The space is very important.This reads left to right because space is present.
  color:red;
}

Here , the text in .title class contained in the div element is coloured red.Something has to be contained in another for this to work.


3. Combined selectors :

selector1.selector2{

}

selector1#selector2{

}

Eg:

h1#title{
  color:red;
}

Here , the h1 which has an ID of title is coloured red.

**WHEN THEIR IS SPACE , THEN IT IS READ FROM LEFT TO RIGHT.IF THEIR IS NO SPACE , READ IT FROM RIGHT TO LEFT.**

--------------------------------------------------------------------------------------------------------------------------

Selector priority in CSS :

Eg 1:
h1{
  color: red;
  color: green;
}
Here , the last CSS rule change is the one that will be carried out.So , h1 becomes green.


.h1_class{
  color:yellow;
}

Now , h1 becomes yellow.This is because classes have a higher ranking in the hierarchical order than html elements.

Similarly , id's have the highest priority over classes and elements.

Also , inline CSS code > ID's.

Note : Use ID's very very sparingly.


-------------------------------------------------------------------------------------------------------------------------


<div class ="container" style="background-color:yellow">
    <p>In HTML, a section is a semantic element for creating
    standalone sections in a web page. These sections should be made up of related
    content, like contact information. The section element should only be used if
    there isn't a more specific element to represent the related content
    </p>
</div>  

Containers allows us to horizontally centre our matter that we want to display.It also automatically
resizes the matter to suit different screens.This makes our content fully responsive.

The class container-fluid can be used to resize the matter to fill 100% of the screen.

The normal container is jumping through the different widths as we change the screen size but the fluid container
resizes the container as we change the screen size to always occupy 100% of the screen width.

------------------------------------------------------------------------------------------------------------------------

 SVGS - Scalable vector graphics:

<!DOCTYPE html>
<html>
<body>

<h1>My first SVG</h1>

<svg width="100" height="100">
   <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
   Sorry, your browser does not support inline SVG.
</svg>

</body>
</html>

SVG stands for Scalable Vector Graphics
SVG is used to define vector-based graphics for the Web
SVG defines the graphics in XML format
Every element and every attribute in SVG files can be animated
SVG is a W3C recommendation
SVG integrates with other W3C standards such as the DOM and XSL

Advantages :

SVG images can be created and edited with any text editor
SVG images can be searched, indexed, scripted, and compressed
SVG images are scalable
SVG images can be printed with high quality at any resolution
SVG images are zoomable
SVG graphics do NOT lose any quality if they are zoomed or resized
SVG is an open standard
SVG files are pure XML


---------------------------------------------------------------------------------------------------------------------
