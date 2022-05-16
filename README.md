# Office 365 
tutorial on how to setup free trial office 365 from microsoft!

## Content table
1. [Sign up in office 365](#Sign-up-in-office-365)
2. [License and applications](#License-and-applications)
3. [Basic setup Azure and GPO](#basic-setup-azure-and-gpo)
    1. 3.1 [Add users and make vm](#add-users-and-setup-vm)
    2. 3.2 [Groups Policy Object](#groups-policy-object)

## Sign up in office 365  
1.Go to [this website here](https://www.microsoft.com/en-us/microsoft-365/microsoft-365-business-standard-one-month-trial) for registration
2. Click the **Big Blue** button
![afbeelding](https://user-images.githubusercontent.com/30397019/168060480-38b8cb16-4857-465d-bc1b-1c236f9d3f06.png)  
3. Microsoft will give the following screen. If you have an existing account you can enter your mail if not, it will make one automaticly for you
![afbeelding](https://user-images.githubusercontent.com/30397019/168062026-408e1592-8383-4b60-ba50-2f2c938807c7.png)  
This is the screen that you will get if you **don't** have an account  
![afbeelding](https://user-images.githubusercontent.com/30397019/168063322-6d737fa3-e1a2-49f5-8817-67f333f657c6.png)  
4. Fill in your information  
![afbeelding](https://user-images.githubusercontent.com/30397019/168065179-8ee413fa-22a2-4053-a30d-5e6514ec23a2.png)  
5. Make sure you have  your phone number filled in for verification
![afbeelding](https://user-images.githubusercontent.com/30397019/168065559-82b056ac-4596-4215-a151-809088d07872.png)  
6. After your sms/phone verification fill in your new "login" information
![afbeelding](https://user-images.githubusercontent.com/30397019/168066385-11382a97-2226-47fa-a6ec-82d7095c6c8d.png)  
7. Put in the quanity you like and press the blue **add payment method** button
![afbeelding](https://user-images.githubusercontent.com/30397019/168066679-60490c43-d1cc-4975-b596-4670bcd94c85.png)  
8. Add your information of your credit card in  
![afbeelding](https://user-images.githubusercontent.com/30397019/168067024-23f4c952-7993-4ddd-91c3-13a94c9166eb.png)  
9. Review your information and edit if necessary, if everthing is filled correct press the blue **start trial** button
![afbeelding](https://user-images.githubusercontent.com/30397019/168068077-1b90c1a6-b3b2-4257-b84e-8ffa8d1f5fed.png)  
9.1. Make sure to read the little text so that you won't be charched for something you don't want
![afbeelding](https://user-images.githubusercontent.com/30397019/168069687-a137bc1b-0f5f-4240-8990-6a3657d070ae.png)  
10. depending on your card/bank/country you may get a prompt for paying.

## License and applications
1. Go to [admin.microsoft.com](https://admin.microsoft.com/)  
You see now the homepage can be empty or can have some tiles in it. You can customize this to your needs. If you like some more Cards press the button add cards. (If you like to change your theme to darkmode press the dark mode button)  
![afbeelding](https://user-images.githubusercontent.com/30397019/168074007-46c938d6-96a8-4056-856e-91a8e3d25915.png)  
Now we are going to get some applications
2. Press on the left side of the screen the button Billing  
![afbeelding](https://user-images.githubusercontent.com/30397019/168074994-396173d1-6ffe-4833-a685-02615aeeed76.png)  
3. press Purchase services
4. Now compare maximum 3 services. (If you already know what service you like to get, check your service on compare and a random other product to "compare")  
![afbeelding](https://user-images.githubusercontent.com/30397019/168075327-46f0bc09-145a-4116-8d5b-9d9b17be36ea.png)  
![afbeelding](https://user-images.githubusercontent.com/30397019/168075674-3851830a-8570-4545-87fe-6a0bbdf91eae.png)  
Press the compare button  
5. Now you can compare if you are still unsure about the different products, if you are ready choose Details  
![afbeelding](https://user-images.githubusercontent.com/30397019/168075897-79bd1677-2cbe-4986-b517-c45ee4dd8dbb.png)  
Now depending on your choice  you get a new comparrison
6. Press details on one of the other products
![afbeelding](https://user-images.githubusercontent.com/30397019/168076522-0dc28ba5-9d25-4b27-888a-e274dd5a8bf1.png)  
You get a new comparison but now there is a button next to buy  
7. Select free trial  
![afbeelding](https://user-images.githubusercontent.com/30397019/168076883-c5e76023-af35-41c7-afb1-3353f5c213ea.png)  
8. Choose your landmark and type in your phone number after you are done choose call me (text me always result in a wrong code) after putting in start free trial  
![afbeelding](https://user-images.githubusercontent.com/30397019/168077324-d9f4bc60-d4c5-45a0-b58b-c2428c4bac3d.png)  
![afbeelding](https://user-images.githubusercontent.com/30397019/168077616-7a27c954-a6f6-4dc1-9574-8903ca20f2f3.png)  
9. Confirm and continue  
![afbeelding](https://user-images.githubusercontent.com/30397019/168077692-64916695-a1e6-4936-a06d-ab2e89890760.png)
![afbeelding](https://user-images.githubusercontent.com/30397019/168078867-b520715e-7ece-4c47-a1f0-6d24622b0cec.png)  

You now have active subscription on your free trial  
![afbeelding](https://user-images.githubusercontent.com/30397019/168080432-d5a83d8f-c938-4b4c-a193-9584690889ab.png)  

# !!don't forget to remove your card if you don't want to be charged for next month after your trial!!  

## Basic setup Azure and GPO
### Add users and setup vm
1. First things first, add your own domain in settings -> domains if you already have one or if you want a custom domain then you can buy one. I am going to use this microsoft default one instead of my own.  
![afbeelding](https://user-images.githubusercontent.com/30397019/168541087-343a8cd8-5ea7-46e4-bd95-989e78b3f873.png)  
2. Now we are going to add some new users, we have different options in here. Go to Users -> Active users. You can now choose to do each individual by pressing add a user or you can add them in bulk by pressing add multiple users at once.  
![afbeelding](https://user-images.githubusercontent.com/30397019/168543480-14a2df8a-6afc-4d61-9656-438d22fb0e80.png)  
everthing is very ez to do.  after you are done making some users, I suggest to make a virtual machine to test your policys to run everthing smoothly.  
I made a test account just for this procedure  
![afbeelding](https://user-images.githubusercontent.com/30397019/168547114-32a79d83-d259-4601-a446-e18562b3b20b.png)  
3. We are now going to install a virtual machine, there are 3 big vm software to run virtual machines [Virtualbox](https://www.pcgamer.com/virtualbox-tutorial/), [Hyper-V](https://www.groovypost.com/howto/create-virtual-machine-windows-10-hyper-v/), [VMware](https://kb.vmware.com/s/article/2128797), choose one of the software you want to use.  
download the microsoft creation tool [here](https://go.microsoft.com/fwlink/?LinkId=691209) open it, accept agreement and then choose the second option Installationmedia.  
![afbeelding](https://user-images.githubusercontent.com/30397019/168550769-a405ded9-110a-408b-9901-b42047f45a6f.png)  
4. Press next and choose your preference. After that is done choose Iso-file(second option) and choose your download location. After that is done you can now use windows 10 with the VM(virtualmachine) to test your things.  
5. Now after your installation is done of windows go to settings -> accounts.  
![afbeelding](https://user-images.githubusercontent.com/30397019/168555239-9688011c-5e6d-4414-9ae3-02405f78ac81.png)  
6. Now press Acces work or school  
![afbeelding](https://user-images.githubusercontent.com/30397019/168555419-aad36957-b882-46a0-b0a8-f54b20e271d9.png)  
7. Press connect and in the new open window press "Join this device to Azure Active Directory"  
![afbeelding](https://user-images.githubusercontent.com/30397019/168555845-fb270749-6095-437a-9b15-8d463e6bc72a.png)  
Enter an e-mail address from your new domain.  
8. After entering the mail and password now press join.
![afbeelding](https://user-images.githubusercontent.com/30397019/168556565-f6e7d808-6250-4ca0-ba14-37760a6d52b6.png)  
9. Good job all set now!! Now you only have to switch accounts.
![afbeelding](https://user-images.githubusercontent.com/30397019/168556850-01b5c8e4-7c0b-4f84-9f08-f79e37959f0d.png)  
10. put in the basic things on your first join. Go to settings and then Update & security. On Activiation you see the activated edition you chose on your trial product. (you can shutdown the machine)  
![afbeelding](https://user-images.githubusercontent.com/30397019/168562445-1ea4ed8a-f9f3-4e25-b767-b606b122cea9.png)  

### Groups Policy Object
Now we are going to edit some basic policys in azure.
1. Go to Endpoint manager  and login.
![afbeelding](https://user-images.githubusercontent.com/30397019/168565085-c8705a0f-bee1-4af4-a3f8-dfdcab04b3d0.png)  
Now you have lots of options for different settings.  
2. Press Devices.  
![afbeelding](https://user-images.githubusercontent.com/30397019/168566753-7666b2b0-2e89-463b-9dd4-451fb3d6ba2d.png)  
3. Press configuration devices  
![afbeelding](https://user-images.githubusercontent.com/30397019/168567065-72c8cdbc-3071-4726-b520-87ea49569207.png)  
And then you can create a profile for your policy  
4. choose your prefered OS(operating system)  
![afbeelding](https://user-images.githubusercontent.com/30397019/168567708-898d2553-fd87-4149-898c-300624286832.png)  
Qua profile type it depends on what you are changing choose one of the 2(I choose settings catalog(prview)).
5. Fill in a unique name in with atleast 4 characters.  
![afbeelding](https://user-images.githubusercontent.com/30397019/168581796-490cc3a0-7dcb-4dd6-abe2-45d2da054235.png)  
(I'm going to set homepage with custom url on edge, very handy for ex a company page.  
6. Press add settings and on the right choose what settings you like to use. (I choose Microsoft Edge -> startup, homepage, ...)  
![afbeelding](https://user-images.githubusercontent.com/30397019/168582367-62cb08eb-d2a2-4a0e-9432-a9f43af43b0b.png)  
The settings I choose are: 
    -Action to take on startup
    -Configure the home page URL
    -Sites to open when the browser starts
7. Press next  
8. choose your groups and/or users and/or devices  
9. Press next 2 times  
10. review and then create and in theory it should work  
![afbeelding](https://user-images.githubusercontent.com/30397019/168583792-b4455904-ec2f-4fcb-878a-9ac9e2ed73b3.png)  



