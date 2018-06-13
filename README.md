# ScrollJS
This is the previous version of an existing repository. The implementation is very easy to achieve, so this version is the best for easy use.

## How to implement?
The implementation is really easy, this is a beginner Javascript file.

* Download or clone this repository

* Add **data-scrollJS** in each link from the menu on another link. The link is added by **ID**, no **Class** atribute.

```
<li>
  <a data-scrollJS href="#about"> About</a>
</li>
```

* Add an ID to the **section** or **DIV** you want to send with the link. For example:

```
<section id="about">
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. 
  Cum voluptatum eum, dicta nihil soluta tenetur repellendus cupiditate quam   perspiciatis nam!</p>
</section>
```

**OR**
```
<div id="about">
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. 
  Expedita voluptates iure aspernatur aut obcaecati veritatis facilis. Odio,   nihil, voluptatibus. At.</p>
</div>
```
* Add **scroll.min.js** on the bottom of your HTML code

```
<script src="js/scroll.js"></script>
```


* After adding **script.min.js** add the following code:
```
<script>
      smoothScroll.init({
      selector: '[data-scrollJS]', // Selector for links, only ID
      selectorHeader: null, // Selector for fixed headers (must be a valid CSS selector) [optional]
      speed: 5000, // Integer. How fast to complete the scroll in milliseconds. By default is 5 seconds.
      easing: 'easeInOutCubic', // Easing pattern to use
      offset: 0, // Integer. How far to offset the scrolling anchor location in pixels
      callback: function ( anchor, toggle ) {} // Function to run after scrolling
      });
</script>
```

And that's it, your code is working


