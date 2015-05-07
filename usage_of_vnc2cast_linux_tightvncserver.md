# Linux with tightvncserver #
  * 1. install VNC server
    * tightvncserver
      * install:
        * sudo apt-get install tightvncserver
      * run:
        * $ vncserver
        * then default VNC port is 5901
      * NOTE:
        * you need websockify for vncserver (Xtightvnc)
  * 2. install websockify
    * download:
      * git clone https://github.com/kanaka/websockify.git
    * run:
      * cd websockify/other
      * make
      * ./websockify 6080 localhost:5901
        * here 5901 is port of your VNC server
          * if needed, you have to change it according to your VNC server's port
        * 6080 is the websockify agent port, which you need to input in vnc2cast
        * websockify is agent between vnc2cast and VNC server
        * you **MUST** run websockify for **vncserver** to let vnc2cast works
      * ![http://pic.yupoo.com/mimepp/EbPLfvJ6/bjKsi.png](http://pic.yupoo.com/mimepp/EbPLfvJ6/bjKsi.png)
  * 3. vnc2cast
    * input the IP address of your VNC server
    * input the port of websockify, e.g.: 6080
    * input the password of your VNC server if you have one
    * press button of "Vnc to chromecast", then chromecast will show screen of your VNC server