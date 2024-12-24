## Camera Absensi

This project is a simple camera attendance system using the webcam.js library. This project is made using the HTML, CSS, and JavaScript programming languages.

## Packages Usage
- WebcamJS v1.0.25


## Installation
1. Clone the repository `git clone
2. Run file index.html in your browser
3. Allow the browser to access the camera
4. Take a photo and the photo will be displayed on the screen
5. The photo will be converted to base64 and can be sent to the database


## Setting WebcamJS Library
- Adjust the width and height of the camera
```javascript
Webcam.set({
    width: 320,
    height: 240,
    image_format: 'jpeg',
    jpeg_quality: 90
});
```
- Documentation: [WebcamJS](https://github.com/jhuckaby/webcamjs)

## Capture Image from Webcam and Display in Page with WebcamJS
- Capture image from webcam
```javascript
  Webcam.snap(function (data_uri) {
    // display results in page
    document.getElementById('results').innerHTML =
        '<img src="' + data_uri + '"/><input type="text" name="foto" value="' + data_uri + '" required/>';
});
```

- Input here decodebase 64 will be converted through php to become PNG when sent to the database.
```html
'<img src="' + data_uri + '"/><input type="text" name="foto" value="' + data_uri + '" required/>';
````

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

