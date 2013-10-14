jQuery DragToEnvoke
==============

Fork of jquery.dragToEnvoke from [Ben Gourley], a draggable jQuery Switch

So what's different?
--------------------
The original script turns a div into a draggable switch. This script is modified to convert (acutally wrap) a checkbox into a draggable switch. The script listens for the change event on the checkbox, so you can programmatically change the state of the switch.

How to use it?
--------------
```javascript
// Setup with default options
$('input[type=checkbox]')
    .dragToEnvoke({
		onFunc : function(el, parent, checkbox) { },
        offFunc : function(el, parent, checkbox) { },
        returnTime : 100,
        balancePoint : 0.5,
        runOnce : false,
        handleText : "",
		defaultState : '' //on or off
	});
```
You can define a default state of the switch by passing it as an option or you can just add the checked attribute to the checkbox.

To change the state programmatically just trigger a click on the checkbox:
```javascript
$('input[type=checkbox]').click();
```
For a demo download the repository and check out demo.html.


License
-------
MIT License


[Ben Gourley]:https://github.com/bengourley/Plugins