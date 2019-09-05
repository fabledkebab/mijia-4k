## MiJia 4K camera research
This is a research repo. It contains some examples of an autoexec file.  
**WARNING: I will be not responsible for any damage you made to your camera!** 

### What do we know
First of all, the camera has an internal server which is semi-web and semi-FTP server.  
Second, it runs Unix-based or Linux-based OS (I am keen on Linux).  
Third, it can execute bash scripts (on boot).  
And that's all for now!  

### How to check the "vulnerabilities"
To check the first one, you need to activate the WiFi hotspot on your camera,
then connect to it using some device. Go to 192.168.42.1 in your browser and
you will see that there is some mysterious web server (actually, it's being used
by the app to communicate with the camera).

The second one can be proven by connecting the camera to your computer using UART
and typing "uname" in terminal.

And the final one can be checked by the same way. Just make an autoexec.ash file in
the root of camera's SD card and then put some "hello world" script, connect by UART
and check what's happening on the camera!  

### Credits
- fabledkebab - the creator of this repo  
- KonradIT - he hacked GoPro Hero cameras  
- and the others one :)  
