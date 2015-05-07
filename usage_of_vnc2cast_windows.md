# Windows #
  * 1. install VNC server
    * You could use one of following VNC servers, I recommend "real vnc"
    * A. real vnc
      * download:
        * https://ww2.chemistry.gatech.edu/software/RealVNC/vnc-4_1_3-x86_win32.zip
        * or google "vnc-4\_1\_3-x86\_win32.zip index of" to download it
      * install:
        * install vnc-4\_1\_3-x86\_win32.exe as a normal windows program
      * run
        * select real vnc server (User-Mode)
        * default VNC port is 5900
        * ![http://pic.yupoo.com/mimepp/EbPLfH4n/GPJe5.jpg](http://pic.yupoo.com/mimepp/EbPLfH4n/GPJe5.jpg)
    * B. tightvnc
      * download:
        * http://www.tightvnc.com/download.php
      * install:
        * install it as a normal windows program
      * run
        * select tight vnc server
        * default VNC port is 5900
        * ![http://pic.yupoo.com/mimepp/EbPLfjoN/KHIrj.jpg](http://pic.yupoo.com/mimepp/EbPLfjoN/KHIrj.jpg)
  * 2. install websockify
    * download:
      * https://github.com/downloads/kanaka/websockify/websockify.zip
    * install:
      * please unzip it to a folder, e.g.: d:\
    * run:
      * run "cmd.exe", change path to the folder of websockify, and run it at port 6080
      * e.g.:
        * C:\Users\top>d:
        * D:\>cd websockify
        * D:\websockify>websockify.exe 6080 localhost:5900
          * here 5900 is port of your VNC server;
            * if needed, you have to change it according to your VNC server's port;
          * **6080** is the websockify agent port, which you need to input in vnc2cast;
    * websockify is agent between vnc2cast and VNC server
      * you **MUST** run websockify on Windows to let vnc2cast works.
    * ![http://pic.yupoo.com/mimepp/EbYuGwMt/FPDpo.png](http://pic.yupoo.com/mimepp/EbYuGwMt/FPDpo.png)
  * 3. vnc2cast
    * input the IP address of your VNC server
    * input the port of websockify, e.g.: 6080
    * input the password of your VNC server if you have one
    * press button of "Vnc to chromecast", then chromecast will show screen of your VNC server