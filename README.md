ETC-EOS Movinglight controls for Streamdeck+

If you havent already, download Companion from this site (https://bitfocus.io/companion)
You can download the stable version of this software. I have not tested this configuration with other builds.

After you have fully installed Companion, make sure all instances of the OEM Streamdeck Software is fully closed on your comptuer. 

When you open up companion you will see the following window;

![Alt text](file:///Screenshot_20230129_021918.png)

You can set your GUI Interface to 127.0.0.1 (Local Host), Port 8000. Click 'Launch GUI'

-Companion First Time Setup- (Configuration Wizard)
You must Enable OSC to port '12321'

Click on 'Connections'

'Image'

On the Right side you will see 'Add Connection'

Search for 'Generic OSC', click add
Search for 'etc-eos', click add

These are the only 2 modules needed for this Config file.

Click Edit on Generic OSC. 

'Image'

Here you can label the OSC Module. 

At this point we need your ETC Nomad IP Address. You will use this for the other module as well. 

-Image-

In this example my ETC IP is 192.168.4.50. Our OSC port is 8001.

To find this information, start up ETC Nomad. In the 'About' section it will tell you you IP Address.
While in Nomad we must also turn on our OSC and make sure our ports are correct.

-Image-

-Image-

After all this is setup, both of your modules should now have a status of 'Ok'

If not make sure your Target IP in each module is correct.

At this point your connections are setup and all we need now is the Config file.

Download the Config file at this URL.

github.com/mbresin

In Companion goto the 'Buttons' Tab, and click 'Import/Export' on the right side.

Click 'Import'

Select the Config File you just downloaded. At this point you should be all setup.
