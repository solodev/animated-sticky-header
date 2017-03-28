# animated-sticky-header
An animated sticky header helps maintain design integrity as your website loads, and yet preserves needed space while providing essential navigation options as a given user scrolls down the page.

A little use of CSS3 transitions provides the subtle animations that interconnect the two header viewpoints. With some additional responsive styling, you'll have a contemporary animated sticky header. 

## Tutorial

For detailed instructions, view Solodev's [Create an Animated Sticky Header](https://www.solodev.com/blog/web-design/create-an-animated-sticky-header.stml) article.

## Demo

Try out a working example on [JSFiddle](https://jsfiddle.net/solodev/5ba7m7hn/).

## HTML

The animated sticky header contains the following basic HTML markup:
```
<header>
  <nav class="navbar navbar-default navbar-fixed-top">

    <div class="navbar-header">
      <div class="container">
        <a class="navbar-brand" href="#">
           <img src="https://www.solodev.com/assets/side-nav/logo.png" alt="Logo Solodev">
        </a>
                        
        <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar" aria-expanded="false" aria-controls="navbar">
          <span class="sr-only">Toggle navigation</span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
        </button>
                        
          </div>
        </div>
        
    <div id="navbar" class="navbar-collapse collapse navbar-right">
      <div class="container">
        <ul class="nav navbar-nav">
          <li><a href="#">Home</a></li>
          <li><a href="#about">About</a></li>
                        <li><a href="#services">Services</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
                <ul class="social">
                  <li><a href="#"><i class="fa fa-facebook" aria-hidden="true"></i></a></li>
                  <li><a href="#"><i class="fa fa-twitter" aria-hidden="true"></i></a></li>
                  <li><a href="#"><i class="fa fa-linkedin" aria-hidden="true"></i></a></li>
                </ul>
          </div>
    </div><!--/.nav-collapse -->

                  
  </nav>
</header>

<div style="display: block; margin: 0 auto; text-align: center;">
  <img class="img-responsive" src="https://www.solodev.com/assets/hero/large-image.jpg">
</div>
```
## CSS

All required CSS can be found in animated-sticky-header.css

## JS

All needed JS is below:
```
$(window).scroll(function() {
    if ($(this).scrollTop() > 1){  
        $('header').addClass("sticky");
    }
    else{
        $('header').removeClass("sticky");
    }
});
```

## External Includes

This tutorial contains the following third party resources.

```
<link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
<link href="animated-sticky-header.css" rel="stylesheet">
<link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
<script src="animated-sticky-header.js"></script>
```
