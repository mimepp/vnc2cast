# Linux #
  * 1. install VNC server
    * x11vnc
      * install:
        * sudo apt-get install x11vnc
      * run:
        * $ x11vnc --forever
        * then default VNC port is 5900
      * NOTE:
        * you do **NOT** need websockify for x11vnc server
        * and in vnc2cast, **the port should be 5900, not 6080**
      * ![http://pic.yupoo.com/mimepp/EbQbqMbn/Ze34E.png](http://pic.yupoo.com/mimepp/EbQbqMbn/Ze34E.png)
  * 2. vnc2cast
    * input the IP address of your VNC server
    * input the port of VNC server, e.g.: 5900
    * input the password of your VNC server if you have one
    * press button of "Vnc to chromecast", then chromecast will show screen of your VNC server

# Linux with tightvncserver #
  * [Linux with tightvncserver](https://code.google.com/p/vnc2cast/wiki/usage_of_vnc2cast_linux_tightvncserver)