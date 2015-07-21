jquery.pleaseWait
--
Displays a "loading spinner" on a given element, intended for use during ajax requests. Does not require any images or css classes, uses a base64 encoded image. Good alternative to a gif for overlaying a spinner on a variety of colored background, as it does not show aliasing around the animated image.

Through options, you can replace the image, adjust the speed, and adjust the interval. Use "crazy" option to spin the target instead of the cog image.

Defaults
--
`````
 $.fn.pleaseWait.defaults = {
  crazy:false,
  speed:8,
  increment: 2,
  image:{base64 encoded image},
  imageType: 'encoded',
  height:65,
  width:65
};
````

Use
--
````
$('#test').pleaseWait(); // starts the waiter
$('#test').pleaseWait('stop'); // stops the waiter
````

Demo
--

http://jsfiddle.net/s7t0saws/

Notes
--
* Be sure to update the width and height if you are replacing the image. The width and height must be to same as the measurement of your replacement image.

* If you are supplying the URL of an image, change imageType to any value other than "encoded".


Key words: please wait, loading animation, loading spinner, ajax spinner, ajax loader, ajax animation, gif alternative
