# jquery.pleaseWait

Displays a spinner on a given element, intended for use during ajax requests. Does not require any images or css classes, uses a base64 encoded image.

Through options, you can replace the image, adjust the speed, and adjust the interval. Use "crazy" option to spin the target instead of the cog image.

Defaults:

`````
 $.fn.pleaseWait.defaults = {
  crazy:false,
  speed:8,
  increment: 2,
  image:{base64 encoded image},
  image_type: 'encoded',
  height:65,
  width:65
};
````

Use:

````
$('#test').pleaseWait(); // starts the waiter
$('#test').pleaseWait('stop'); // stops the waiter
````
