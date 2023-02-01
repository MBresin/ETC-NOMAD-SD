ETC-EOS Movinglight controls for Streamdeck+

If you havent already, download Companion from this site (https://bitfocus.io/companion)
You can download the stable version of this software. I have not tested this configuration with other builds.

After you have fully installed Companion, make sure all instances of the OEM Streamdeck Software is fully closed on your comptuer. 

When you open up companion you will see the following window;

<img width="402" alt="image" src="https://user-images.githubusercontent.com/121821262/216143119-69601c92-1017-45fe-8d3d-2e21c2dca8ba.png">

You can set your GUI Interface to 127.0.0.1 (Local Host), Port 8000. Click 'Launch GUI'

-Companion First Time Setup- (Configuration Wizard)
You must Enable OSC to port '12321'

Click on 'Connections'

<img width="1379" alt="image" src="https://user-images.githubusercontent.com/121821262/216143246-73445511-02c8-42ab-98bb-4fe62529c2fa.png">


On the Right side you will see 'Add Connection'

Search for 'Generic OSC', click add
Search for 'etc-eos', click add

These are the only 2 modules needed for this Config file.

Click Edit on Generic OSC. 

<img width="1380" alt="image" src="https://user-images.githubusercontent.com/121821262/216143373-94205373-b76e-4b55-80be-72deb7f0cf31.png">

Here you can label the OSC Module. 

At this point we need your ETC Nomad IP Address. You will use this for the other module as well. 

In this example my ETC IP is 192.168.4.50. Our OSC port is 8001.

To find this information, start up ETC Nomad. In the 'About' section it will tell you you IP Address.
While in Nomad we must also turn on our OSC and make sure our ports are correct.

<img width="1149" alt="Screenshot 2023-02-01 at 2 29 22 PM" src="https://user-images.githubusercontent.com/121821262/216143976-92ea6fcf-e548-4e34-b0f5-8b3d104c5c11.png">

After all this setup, both of your modules should now have a status of 'Ok'

If not make sure your Target IP in each module is correct.

<img width="522" alt="Screenshot 2023-02-01 at 1 57 23 PM" src="https://user-images.githubusercontent.com/121821262/216144500-3f41e90f-cac4-49cf-b3e2-ca8e47e09c58.png">

At this point your connections are setup and all we need now is the Config file.

Download the Config file at this URL.

github.com/mbresin

On YOur Console (Nomad) you need to setup your OSC Connections. In Setup/Show Control/OSC. Set your RX Port to 8001, your TX port to 12321

<img width="970" alt="Screenshot 2023-02-01 at 2 15 46 PM" src="https://user-images.githubusercontent.com/121821262/216145390-9daa8671-f568-449b-95a0-6f1eb011bcb0.png">


In Companion goto the 'Buttons' Tab, and click 'Import/Export' on the right side.

<img width="536" alt="Screenshot 2023-02-01 at 2 00 11 PM" src="https://user-images.githubusercontent.com/121821262/216144721-10eaac95-e48f-44d0-81c4-5704abc14e89.png">

Click 'Import'

Select the Config File you just downloaded. At this point you should be all setup.

If your having issues connecting your surface try rescaning for USB.

<img width="1364" alt="Screenshot 2023-02-01 at 1 59 59 PM" src="https://user-images.githubusercontent.com/121821262/216145782-1d4f43f6-c709-4a27-996d-9e275560a3c9.png">

etc-eos Module issues, always double check your ip matches the console in the module. It needs to be the Target IP.

