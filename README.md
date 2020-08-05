# simple-ui

## Overview

A simple graphical UI to execute JavaScript

## Usage

Open <https://takanori-pskq.github.io/simple-ui/> to create a new UI page. Here you can edit the page title and the actions of each button. Scripts are written in JavaScript.

The URL of the generated page is like `https://takanori-pskq.github.io/simple-ui/ui?config=xxxxxx`, and `config` parameter (`xxxxxx`) is a JSON string which is URL encoded after base64 encoded. This includes all the settings and actions. Here is the structure of the JSON:
```
{
	"title": "Page Title"
	"onload": "Script for initialize"
	"buttons": [
		{
			"label": "Label of button1",
			"onclick": "Script for actions of button1"
		}, {
			"label": "Label of button2",
			"onclick": "Script for actions of button2"
		}, ...
	}
}
```
So you can generate a URL of the page without generator.

## License

MIT License
