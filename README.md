# twilio-js
  
  A port of TwilioCapability from [twilio-python](https://github.com/twilio/twilio-python) to Javascript.
  Useful for generating Twilio Client tokens purely client side, e.g. Google Chrome extensions.
  
     var capability = new TwilioCapability(ACCOUNT_SID, AUTH_TOKEN);
     capability.allow_client_incoming('matt');
     capability.allow_client_outgoing(APP_SID, 'matt');
     var token = capability.generate();

     Twilio.Device.setup(token);

## Build
  
  Java is required to minify the build, and Google Closure will download automatically.
  
     $ make
  
  Clean up (Doesn't remove downloaded Google Closure)!
  
     $ make clean
  
  Clean everything (Including Google Closure):
  
     $ make cleanall

## Known Issues
  
  * _none_

## License 

(The MIT License)

Copyright (c) 2011 Matt Robenolt &lt;root@drund.com&gt;

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
