Install Visual Studio Code

Upload this file to your Arduino:
https://github.com/firmata/arduino/blob/master/examples/StandardFirmataPlus/StandardFirmataPlus.ino

And change the usb port in `app.js`

in your terminal navigate to the directory you want to use
type : `git clone https://github.com/thomassr/hackathon-master-digital-design`

then `cd hackathon-master-digital-design`
then `npm install`
then `npm run serve`

in `app.js` you can change the value of when 'explode' triggers
Where `i` equals the amount of buttons pressed.
```javascript
if (i >= 10) {
    console.log('Explosion');
    //Sends the explode command to the client
    socket.emit('explode');
    i = 0;
}
```

in `main.js` change 	
```javascript
console.log('explosion!!');
	
document.querySelector('.sun').style = "transform: scale(1.2);"
```

To the call of the particle function.
