DEPRECATION WARNING
===================
This plugin is UNMAINTAINED and has not been updated since 2013. Please do not ask for help in the Issues section as I will not be able to help you!

MediaScannerPlugin
============

This plugin invokes the Media Scanner on Android OS to add media files to the device's Media Index. If you download an image or a video, you will need to use the Media Scanner to index it before it will show up in the Android Gallery. This plugin will allow you to do that.

Installation
------------

### For Cordova 3.0.x:

1. To add this plugin just type: `cordova plugin add https://github.com/peteygao/MediaScannerPlugin.git` or `phonegap local plugin add https://github.com/peteygao/MediaScannerPlugin.git`
2. To remove this plugin type: `cordova plugin remove org.sfl.MediaScannerPlugin` or `phonegap local plugin remove org.sfl.MediaScannerPlugin`


Usage:
------

Call the `window.MediaScannerPlugin(successCallback, failureCallback)` method by passing in your success and error callbacks:

### Example
```javascript
function onDeviceReady()
{
	window.MediaScannerPlugin.scanFile(
        function(msg){
            console.log(msg);
        },
        function(err){
            console.log(err);
        }
    );
}
```

The function will call your successCallback upon success, and failureCallback on failure.

## License

The MIT License

Copyright (c) 2013 Peter Gao (http://github.com/peteygao)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Special Thanks
Tommy-Carlos Williams (https://github.com/devgeeks/Canvas2ImagePlugin)

Joseph Khan (https://jbkflex.wordpress.com/2012/12/23/saving-image-to-android-devices-gallery-phonegap-android/)
