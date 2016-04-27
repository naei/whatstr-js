## whatstr.js

A JavaScript library to watch for typed chars, being based on browser behavior instead of keyCode. Also provide a human readable way to get commons typed commands within a webpage. It has no dependencies.

### Usage

###### Watch for text inputs:

```javascript
whatstr.onTextInput (
	// callback function
	function(char){
		// log the typed char
		console.log(char);
	},
	// optional - specify an element to watch (must be a text input)
	// if null or empty, all the activity on the webpage is watched
	document.getElementById('a-text-input')
);
```

###### Watch for commands:

```javascript
whatstr.onCmdInput(
    // callback function
	function(cmd){
		// log an array of strings of the typed command
  		console.log(cmd);
	},
	// optional - if set to true, will prevent some shortcuts to be executed
	true
);
```

### Notice

Copyright (c) 2016 Lucas Pantanella

The sources are released under the terms of the [MIT license](LICENSE).
