# **_<center>Raspberry Pi Documentation</center>_**

---

## **_So what is Raspberry Pi?_**

>The Raspberry Pi is a very cheap computer that runs Linux, but it also provides a set
of GPIO (general purpose input/output) pins,
allowing you to control electronic components for
physical computing and explore the Internet of Things (IoT).

### _**Step 1:**_ Install Headless **Raspbian OS** into _Raspberry Pi_
 _(https://www.raspberrypi.com/software/)_

 - Raspberry Pi Imager is the quick and easy way to install Raspberry Pi OS and other operating systems to a microSD card, ready to use with your Raspberry Pi.
 Here is the link for the [Raspberry Pi Imager](https://www.raspberrypi.com/software/)
 ![Screenshot 2023-12-07 145420](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/e2574685-2757-4d49-a721-188f7f518d8a)

 - Open Raspberry Pi Imager. Choose Raspberrry Pi Device, Operating System, and Storage.
 ![Screenshot 2023-12-07 135408](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/ca526d3e-fe83-4ab8-bef8-6a7b401f41e4)

 - In this project, we choose **_Raspberry Pi 3_** as device, **_Raspberry Pi OS (Legacy)_** as operating system, and our **_32GB SD Card_** as storage.
 ![Screenshot 2023-12-07 135512](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/9e5fe390-dc24-4570-9de6-0588a0fa450a)
 ![Screenshot 2023-12-07 135541](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/5d91f9da-4a42-40e0-a2b4-148fe5e9640d)
 ![Screenshot 2023-12-07 135558](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/95cc7542-6144-4873-b516-4fb3a3f675a0)

 - After choosing the preferred device, OS, and storage, click **Next**.
 ![Screenshot 2023-12-07 135616](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/15ea5bcb-cfd5-4235-8742-77087116cb53)

 - ...and click **Edit Settings** to customize the OS Settings.
 ![Screenshot 2023-12-07 135634](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/d99d262e-2f36-4056-9eb7-4661712a5f01)

 - In the OS Customization, we set the host, username, and password as **group1**. We configure our wireless LAN available which is **CSPC BayanihanNet** and set the wireless LAN   country to **PH.** Lastly, we set our timezone to **Asia/Shanghai** since they have the same timezone (GMT+8) with Manila, then click **Save**.
   
 ![Screenshot 2023-12-07 135752](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/d4dc817d-04e5-49c0-831c-e9bda0386683)

 - Don't forget to enable SSH and use password authentication, then click **Save**.
 ![Screenshot 2023-12-07 135810](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/8f8dd69e-c5e5-44f0-a515-b23864ae8db8)

 - Click **Yes** to apply our customized settings.
   ![Screenshot 2023-12-07 140959](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/b1f04a91-fa82-44d9-ae70-e237221f1837)

 > [!WARNING]
 > Make sure to backup all existing data in the SD card to avoid deletion while formatting.
 - A warning will appear that all existing data on our SD card will be erased if we continue on our installation. Click **Yes** since our SD card have no existing files that needs to be backed up.
  ![Screenshot 2023-12-07 135833](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/5378f87f-03f9-45ab-a6c3-e25cba283b61)

 - OS writing on our SD card will then start

![Screenshot 2023-12-07 135844](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/c75ec2ca-df1e-4e13-9766-88eadc471491)

![Screenshot 2023-12-07 135942](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/e8c848b2-cafc-4923-a4c2-77301fdccd3a)

 - After writing, verification will start.
  
![Screenshot 2023-12-07 140853](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/9e465d13-36c9-4316-ba62-5fdd8aafb04c)

 - Wait until the verification hits 100%, and write succesfull prompt will appear. In this part, it's now safe to eject our SD card from the PC.

![Screenshot 2023-12-07 140905](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/33d244ad-11b9-401e-a302-57ad6fb60c1f)

 _**Step 2:**_ Connect to Raspberry Pi via SSH then update the OS
 
**_ssh_** _username@hostname_

**sudo** apt update

**sudo** apt upgrade

 _**Step 3:**_ Install LAMP Stack
 _(https://ostechnix.com/install-apache-mysql-php-lamp-stack-on-ubuntu-18-04-lts/)_
 _(https://linuxhint.com/install-phpmyadmin-raspberry-pi/)_
 
**sudo** _apt install apache2<b>_

**sudo** apt _install mariadb-server_

**sudo** _mysql_secure_installation_

**sudo** _apt install php libapache2-mod-php php-mysql_

**sudo** _apt-get install php*_

**sudo** _apt install phpmyadmin_

 _**Step 4:**_ Connect to _Raspberry Pi via VNC_

**sudo** raspi-config

 _(https://www.realvnc.com/en/connect/download/viewer/)_





