# Slide_Show

## A small Project in which I used JavaScript and Css to create a simple Responsiv Slide show.

![pic1](https://user-images.githubusercontent.com/57542570/154819606-91019c7c-09c6-4863-b511-c67947996ae5.png)



<br><br>
 
 ```JavaScript
var index = 0;

show_slide = (i) => {
  index += i;

  var images = document.getElementsByClassName("image");
  var dots = document.getElementsByClassName("dot");

  // hide all the images
  for (i = 0; i < images.length; i++) 
    images[i].style.display = "none";
  
  // remove the active class from the dot
  for (i = 0; i < dots.length; i++) 
    dots[i].className = dots[i].className.replace(" active", "");
  
  if (index > images.length - 1) 
    index = 0 ;
  
  if (index < 0)
    index = images.length - 1;

  images[index].style.display = "block";
  dots[index].className += " active";

}

window.addEventListener("onload", show_slide(index));
```


### Built With


* [Css](https://wiki.selfhtml.org/wiki/CSS)
* [javaScript](https://developer.mozilla.org/de/docs/Web/JavaScript/)

![pic2](https://user-images.githubusercontent.com/57542570/154819610-132b75a5-0363-4929-92a0-301086cff4d8.png)



<!-- CONTACT -->
## Contact

Meik Grünholz -  prt3@hotmail.de
