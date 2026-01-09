Hours Completed: 4.5 hours

Today, I provisioned a total of 10 phones with Lili for the SFM clinic. The steps were simple; connect phone to PoE, set up wireless connection, print out their extension number and stick the label onto the phones, and pack them back into the box. The longest part was waiting for each phone to receive its configuration and extension. 

After that, it was checking emails and waiting for a help desk call with a different System Analyst (Cam). One popped up. 

I got to go on a site visit to the Blaine FCN clinic. The initial issue was that the credit card reader was not authorizing collecting payments from patients and the purpose of visiting would be to replace the credit card reader itself. When we (Alex and I) got there, we unplugged the old card reader and plugged in the IT loaner one. When we had the receptionist try to collect the payment, it showed an error, something similar to the device not being able to check a specific .dll file.

Then, we checked device manager (shows that device is connected), device drivers (drivers were already updated to latest), and Windows Updates (no new updates) but it seemed like they weren't the issue. So we escalated by asking another System Analyst (Cam) for a different perspective. They decided on uninstalling and reinstalling the credit card reader drivers through the NinjaOne application which allowed Cam to remote into the computer and apply the policy. 
We rebooted the computer after doing the reinstall. He opened the Epic application from the desktop and received the same issue, but then he opened it on the FCN storefront which is connected to the Citrix application and the credit card reader was able to authorize a faux credit card payment.

We had the receptionist test on her account and it was able to authorize the collection payment! Yay. 

Our understanding of what fixed the problem was the difference between using the EPIC Hyperspace locally or online. So understanding how the infrastructure of how everything was interconnected.  

Afterwards, I got a clinic tour and also helped someone learn how to access the label printer in their office. It was quick and simple. 



