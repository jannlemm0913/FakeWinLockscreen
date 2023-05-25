# FakeWinLockscreen
A quick and dirty implementation of a fake Windows 10 lockscreen as a web page.  
This is only intended to be used in awareness trainings or red teaming operations.

When the user left-clicks, the login mask is displayed. Right-clicking hides the login mask again and returns to the idle screen with the clock.  
In this version, if the user enters a password, the browser is redirected to https://avantguard.io/en/homepage. The password is not included in the request.  
Since this was only a small hacky project made for fun, only English is implemented. If you would like to contribute additional languages, please do so!  

![grafik](https://github.com/jannlemm0913/FakeWinLockscreen/assets/37586835/a29e4fe2-51bb-4955-8c33-b038c9c20e16)

Due to CORS, it was not possible to get different images and their respective texts. The API endpoint for that can be found in form.js. With a web server, this could be implemented pretty easily.

### Credits
Some code has been taken from [StephenMcVicker/HTML-Login-Form](https://github.com/StephenMcVicker/HTML-Login-Form)  
Also, check out [Pickfordmatt/SharpLocker](https://github.com/Pickfordmatt/SharpLocker) and its newer implementations. As they are executables, they can get more information (such as the user name) from the current user and more accurately simulate the real lockscreen. However, it is a lot easier to just browse to a known URL on an unlocked workstation than downloading and running an executable... :wink:
