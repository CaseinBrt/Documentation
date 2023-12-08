# **Information Assurance**
---
### Group-12
- _Bayos, Roberto Jr. B._
- _Nadal, Johben A._
- _Gava, John Christian M._

---

## **_<center>Raspberry Pi Documentation</center>_**

---

### **_So, what is Raspberry Pi?_**

>The Raspberry Pi is a very cheap computer that runs Linux, but it also provides a set
of GPIO (general purpose input/output) pins,
allowing you to control electronic components for
physical computing and explore the Internet of Things (IoT).

#### _**Step 1:**_ Install Headless **Raspbian OS** into _Raspberry Pi_
 _(https://www.raspberrypi.com/software/)_

 - First, we need to download and install the **"Raspberry Pi"**
 Here is the link for the [Raspberry Pi Imager](https://www.raspberrypi.com/software/)
 ![400494685_1520571618518673_7952891577700257049_n](https://github.com/CaseinBrt/Documentation/assets/145450481/fb4c181b-9ec7-4383-b793-530b62c4e77c)

 - In this part open the Raspberry Pi Imager, and Choose Raspberrry Pi Device, Operating System, and Storage.
 ![RB](https://github.com/CaseinBrt/Documentation/assets/145450481/96838abe-5998-42f0-b63c-5e96b749a3d3)


 - We choose **Raspberry Pi 3** as device, and **_Raspberry Pi OS (Legacy)_** as operating system. Also, our **32GB SD Card** as storage.
 ![393145357_897420492051420_6817004208116354603_n](https://github.com/CaseinBrt/Documentation/assets/145450481/eea45364-cd29-4005-a12e-86c75f623272)
 ![377241562_1062921111715927_103322438306499714_n](https://github.com/CaseinBrt/Documentation/assets/145450481/c21bc8f7-29f1-41ec-bf69-d7a13772c793)
 ![403411511_412139751467171_3308658335017623501_n](https://github.com/CaseinBrt/Documentation/assets/145450481/90fbd844-8563-4e53-93f3-bf436f8d3e4b)

 - Click **_Next_**. After choosing the device, OS, and storage.
 ![400621530_1335577220401316_8795652795261815842_n](https://github.com/CaseinBrt/Documentation/assets/145450481/ba700896-a09e-4e6f-a8f8-d2334c6362de)


 - To customize the OS Settings, click **EDIT SETTINGS** button.
 ![393194299_363645859540214_7154670965270395864_n](https://github.com/CaseinBrt/Documentation/assets/145450481/f3fa41fd-20a0-4cb9-91d3-0208f6fcb750)

 - In the OS Customization, we set the host, username, and password as **_group12_**. We made some changes in our wireless LAN which is **CSPC BayanihanNet** and set the wireless LAN country to **_PH._** Lastly, we set our timezone to **Asia/Manila** then click **_Save_**.
 ![393114535_1095928151312852_5876205805852913922_n](https://github.com/CaseinBrt/Documentation/assets/145450481/817653fe-8266-4dd7-a384-bb3c67dca0fd)

 - Make sure to enable **"SSH"** and use password authentication, and after that, just click on **Save** button below.
 ![Screenshot 2023-12-07 135810](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/8f8dd69e-c5e5-44f0-a515-b23864ae8db8)

 > All existing data in the SD card make sure to backup to avoid deletion while formatting.
 - A warning will appear reminds the user that all existing data on our SD card will be erased if we continue on our installation.
 - Click **Yes** since our memory card has no existing files.
  ![371472973_1035315564368265_4510458628948484002_n](https://github.com/CaseinBrt/Documentation/assets/145450481/6e7c7ab2-a9b9-4ab0-aa99-83bd6591c74e)

 - OS writing on our SD card will then start...
  ![398353951_2441013162753240_2785452117252676937_n](https://github.com/CaseinBrt/Documentation/assets/145450481/906a36d5-f26e-4f31-9552-1b3e2ae0fd34)

 - The verification will start after writing.
  ![405249132_333825012612138_1117697920856273851_n](https://github.com/CaseinBrt/Documentation/assets/145450481/929d2a27-ddfa-4bdd-8900-2c7c62f66509)

 - Wait until the verification hits 100%, and write succesfull prompt will appear. In this part, it's now safe to eject our SD card from the PC.
 ![377147723_325086653638346_8268673517986389737_n](https://github.com/CaseinBrt/Documentation/assets/145450481/109268e6-f898-43c4-969b-05a48cd369d1)

### 2. Connect to Raspberry Pi via SSH (Secure Socket Shell) then update the OS ###
 - In the command prompt, type SSH to access the network protocol. Then type the following command:
   - ssh username@hostname (e.g. group1@group1)
   - sudo apt update
   - sudo apt upgrade

 ![2(1)](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/a105c0e9-650b-4103-b8b2-03f07588c171)
 
 ![3](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/2bd078ad-1d70-44a7-9209-68f742ac4425)

### 3. Install LAMP Stack. LAMP stands for Linux, Apache, MySQL, and PHP. 
 - This stack is typically installed together in order to enable a server to host dynamic websites and web apps written in PHP.
Here are the tutorials on how to install LAMP stack [[1]](https://ostechnix.com/install-apache-mysql-php-lamp-stack-on-ubuntu-18-04-lts/)[[2]](https://linuxhint.com/install-phpmyadmin-raspberry-pi/)
 - To install the stack, type the following commands on our command prompt connected to Raspberry Pia via SSH.
   + **_sudo apt install apache2_**
     ![4 1](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/0b82373e-fbfe-4572-8fcd-dfe0758f123c)
   + **_sudo apt install mariadb-server_**
     ![5 1](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/e7b4c2e9-88a2-45f9-a672-dcc3fe3a9b45)
   + **_sudo mysql_secure_installation_**
     ![6 1](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/468ada53-65e1-4321-abd0-a0b4fd3a479f)
   + **_sudo apt install php libapache2-mod-php php-mysql_**
     ![7 1](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/fc1b5ee6-b857-46ea-bee6-34b3fc01a40d)
   + **_sudo apt-get install php_**
     ![8](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/7df70005-43fa-4811-8b08-3ffa124a92c4)
   + sudo apt install phpmyadmin
     ![9](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/2f41ba4e-7455-48b4-8e6d-bfa89566ab4a)

### 4. Connect to Raspberry Pi via VNC
 - Install RealVNC® Viewer to the device you want to control from via this [link](https://www.realvnc.com/en/connect/download/viewer/)
 - Before opening VNC on our PC, access first the Raspberry Pi Configuration Tool to enable VNC on the OS via the **_sudo raspi-config_** command.
 - Using the arrows, navigate to **'Interfacing Options'** > **'VNC'**, then choose **'Yes'** and select **'OK'** 
    ![10](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/85362fe9-0d18-4b24-9aec-d6f09b7ebd34)
    ![11](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/d84694be-b952-497a-aa6b-dabb42637f1e)
    ![12](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/5353298f-e2ed-4100-9b13-a810158868bb)
    ![13](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/b4f418d4-fd99-468c-95d8-3c4560da19ae)
- On the device you will use to take control, run RealVNC Viewer and enter the private IP address in the search bar. If the screen of the Raspberry Pi appeared on RealVNC, it means that it already established connection and control on the Raspberry Pi. 
   ![15](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/323d006d-f178-412f-bacc-375844c40927)


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





