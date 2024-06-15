# Setting up and creating our Windows Server 2019 VM

<h1>Summary</h1>
In this lab I will download all required programs and files to create Virtual Machines. We will create our VM's via Virtual Box. We will also download 2 ISO's. One for our Windows Server VM and another for our Windows 10 VM. Finally We will configure our Windows Server 2019 VM 

<h1>Step 1) Downloading Virtual Box </h1>

<img width="188" alt="Screenshot 2024-06-15 at 11 40 22 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/b2d1575b-5f5d-4711-b880-4d7f70a3fb08">

<h2>About Virtual Box</h2>

VirtualBox is a program created by Oracle that allows us to create VM's with different Operating Systems. With the power of Virtual Box I am able to create Windows VM's on my Macbook. We can create and manage multiple VM's with any operating system we would like



1A) Navigate to https://www.virtualbox.org/ and click on the large download virtual box button.

<img width="1790" alt="Screenshot 2024-05-18 at 9 11 41 PM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/52582e31-9258-4323-bcf4-169284ad8815">


<h1>Step 2) Downloading Windows ISO's</h1>

<img width="310" alt="Screenshot 2024-06-15 at 11 48 27 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/8e5d93af-2213-4fd8-a204-955e8210d1fa">

<h2>Summary</h2>

In order for us to create a VM with Virtual Box we need to provide an Operating System. By downloading these ISO's we can provide Virtual Box with different Operating Systems to use


<h2>2A) Downloading the Windows 2019 Server ISO</h2>

Navigate to https://www.microsoft.com/en-us/evalcenter/download-windows-server-2019 and download the 64 bit ISO.

<img width="934" alt="Screenshot 2024-05-19 at 8 00 20 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/a1df45d9-282e-474d-8509-0e4a79d75663">

<h2>2B) Downloading the Windows 10 Enterprise VM</h2>

 Navigate to https://www.microsoft.com/en-us/evalcenter/evaluate-windows-10-enterprise and click on the Download the ISO - Enterprise link.

<img width="1317" alt="Screenshot 2024-05-19 at 8 09 32 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/e5397eca-b6d1-441d-926c-b592f5466ecf">

<h1>Step 3) Creating a Windows 2019 Server VM</h1>
<h2>Summary</h2>

In this step we will go through the steps to create a Windows 2019 VM in virtual box. Note I have already created many VM's so your screen may look different. 
<h2>3A) Open Virtual Box </h2>
<img width="793" alt="Screenshot 2024-05-19 at 8 14 43 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/61643e7d-f3c4-4fce-a1f9-36573b436928">

<h2> 3B) To create our Windows Server virtual machine we are going to click on the big blue button on the top that says new. </h2>

This Virtual Machine will act as our Domain Controller so I have chosen to name it DC. You can name it anything you want just remember what you named it as it is the most important VM we will create.

When selecting the ISO image you will get confirmation that you chose the correct ISO by the version bar on the bottom of the form. If it does not say Windows 2019 (64-bit) then you have selected the wrong ISO.

You may then click Next when you have confirmed everything is correct

Then we are going to click the checkmark for skip unattended installation

<img width="950" alt="Screenshot 2024-05-19 at 12 38 08 PM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/6124e164-4432-4cca-a2eb-c2783c12037a">

Once your screen looks like this you are ready to click next


<h2>3C) Allotting resources</h2>

What we select here is dependent on the power of our CPU and the amount of RAM we have on our system.

I recommend you use at least 4096 MB or roughly 4 GB. This means to run 2 VM's you will ideally need more than 8GB of RAM on your device. If you do not have at least 8GB of RAM then I would lower the number so that your system can handle running 2 VM's at a time.

The Processor also is dependent on your system. If you have a weaker CPU you may just be able to use 1 CPU but for me I will select 3.

Note: You can change these settings once the VM is created by right clicking on the VM and clicking settings.


<img width="947" alt="Screenshot 2024-05-19 at 10 17 17 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/d4fc3415-428d-44c6-b0d5-65140296fc5c">

Once you have chosen your settings you are ready to hit next.

<h2>3C) Alotting Storage</h2>

Now We will allot memory to Our VM. For our purpose 50 GB is fine

<img width="949" alt="Screenshot 2024-05-19 at 10 20 29 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/769d171e-350d-4648-8466-ac3da2e29d40">

<h2>3D) Summary of VM</h2>

 We will now be prompted to review the specifications of the VM we have created
 
<img width="950" alt="Screenshot 2024-05-19 at 10 22 00 AM" src="https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s/assets/66844406/fc6c7676-f8ea-4c36-812b-3f01682e91b9">

We can click the finish button

<h2>3E) Allowing VM to use our home network </h2>


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






