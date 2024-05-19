# Setting up and creating our Windows Server 2019 VM
We are going to download everything required to run windows 10 and windows server 2019. We will also create our Windows Server 2019 Virtual machine.


Step 1) Navigate to https://www.virtualbox.org/ and click on the large download virtual box button.

<img width="1790" alt="Screenshot 2024-05-18 at 9 11 41 PM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/52582e31-9258-4323-bcf4-169284ad8815">



Step 2) Navigate to https://www.microsoft.com/en-us/evalcenter/download-windows-server-2019 and download the 64 bit ISO.



<img width="934" alt="Screenshot 2024-05-19 at 8 00 20 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/a1df45d9-282e-474d-8509-0e4a79d75663">

Step 3) Now that we have our server we need to download Windows 10 so our windows server has users to manage. To do this you will navigate to https://www.microsoft.com/en-us/evalcenter/evaluate-windows-10-enterprise and click on the Download the ISO - Enterprise link.

<img width="1317" alt="Screenshot 2024-05-19 at 8 09 32 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/e5397eca-b6d1-441d-926c-b592f5466ecf">

Step 4) Once you have installed Virtual Box you can open the application and you should see something like this. I have already created a lab environment so the left side of your screen should look different
<img width="793" alt="Screenshot 2024-05-19 at 8 14 43 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/61643e7d-f3c4-4fce-a1f9-36573b436928">

Step 5) To create our Windows Server virtual machine we are going to click on the big blue button on the top that says new. 

<img width="941" alt="Screenshot 2024-05-19 at 8 22 04 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/c7c70579-ceae-4726-97b9-5bc5dff81950">

This Virtual Machine is going to act as our Domain Controller so I have chosen to name it DC. You can name it anything you want just remember what you named it as it is the most important VM we will create.

When selecting the ISO image you will get confirmation that you chose the correct ISO by the version bar on the bottom of the form. If it does not say Windows 2019 (64-bit) then you have selected the wrong ISO.

You may then click Next when you have confirmed everything is correct

Then we are going to click the checkmark for skip unattended installation

<img width="950" alt="Screenshot 2024-05-19 at 12 38 08 PM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/6124e164-4432-4cca-a2eb-c2783c12037a">

Once your screen looks like this you are ready to click next


Step 6) After clicking Next you should see a screen that looks like this

<img width="949" alt="Screenshot 2024-05-19 at 8 43 42 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/909b0146-e84c-487e-8ca6-cbd8432041c3">

What we select here is dependent on the power of our CPU and the amount of RAM we have on our system.

I recommend you use at least 4096 MB or roughly 4 GB. This means to run 2 VM's you will ideally need more than 8GB of RAM on your device. If you do not have at least 8GB of RAM then I would lower the number so that your system can handle running 2 VM's at a time.

The Processor also is dependent on your system. If you have a weaker CPU you may just be able to use 1 CPU but for me I will select 3.

Note: You can change these settings once the VM is created by right clicking on ////

<img width="947" alt="Screenshot 2024-05-19 at 10 17 17 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/d4fc3415-428d-44c6-b0d5-65140296fc5c">

Once you have chosen your settings you are ready to hit next.

Step 7) Next you will be prompted with this screen.

<img width="949" alt="Screenshot 2024-05-19 at 10 20 29 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/769d171e-350d-4648-8466-ac3da2e29d40">

For our purposes this will work so we can go ahead and click Next

 We will then get a summary of the VM we are creating
 
<img width="950" alt="Screenshot 2024-05-19 at 10 22 00 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/fc6c7676-f8ea-4c36-812b-3f01682e91b9">

We can click the finish button

Step 8) Congratulations! You just created your Windows Server 2019 VM!

But before we can start up our machine there's a few things we must do so our system will run properly


We must change some settings so our device boots correctly.

First right click on the VM we just created and select settings...

<img width="379" alt="Screenshot 2024-05-19 at 12 44 37 PM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/61ec8b50-2957-4796-8372-6001fa810011">

You should then see this. Here we could change our VM's name if we wanted to
<img width="695" alt="Screenshot 2024-05-19 at 12 47 27 PM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/e355079d-c1bc-4095-86ec-f45ce3bba891">

We don't want to do that right, instead we are going to click on system
<img width="682" alt="Screenshot 2024-05-19 at 12 49 22 PM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/183675a8-9ba1-4008-9ef4-96d5824b33fb">

We are then going to unselect the floppy checkmark in the boot order
<img width="692" alt="Screenshot 2024-05-19 at 12 50 40 PM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/510e62b8-a405-4c5e-aec2-de55dbdedd7d">

From there select Network on the same menu that we changed our system settings from

<img width="692" alt="Screenshot 2024-05-19 at 12 52 24 PM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/3b855669-62d0-4bcb-9073-6d2a5d597517">

We are then going to change our NAT option into a bridged Adapter. This allows our virtual machine to connect to our home network 
<img width="695" alt="Screenshot 2024-05-19 at 12 53 23 PM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/24a80487-6ae9-4630-bcb6-a026cf36e06d">

Once you have completed that you can click OK and with that we are ready to start using our Windows Server 2019 VM!






