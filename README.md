# MMM-QRCode
QRCode module for MagicMirror². Show QRCode image of encoded text.

## Screenshot
![](.github/example.png)

## Installation
Open up your terminal and paste the following code.
```
cd ~/MagicMirror/modules/
git clone https://github.com/MarinescuEvghenii/MMM-QRCode.git
cd MMM-QRCode && npm i
```
## Using the module

To use this module, add it to the modules array in the `config/config.js` file:
````javascript
{
	module: 'MMM-QRCode',
	config: {
		// See 'Configuration options' for more information.
		text: 'Some Text', // your message
		showRaw: true, // true = to diaplay raw text, false = to hide raw text
		imageSize: 150, // size including both width and heigth
		colorDark: "#fff", // qrcode pixels color to display
		colorLight: "#000" // set background color of qrcode
	}
}
````

## Configuration options

The following property can be configured:

| Option     | Description             | Default value |
| -----------|-------------------------|:-------------:|
| colorDark  | Draw color              | "#fff"        |
| colorLight | Background color        | "#000"        |
| imageSize  | Size of the image in px | 150           |
| showRaw    | Show raw text           | true          |
| text       | The text to be encoded  |               |
