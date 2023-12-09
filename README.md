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

 ---

### _**Step 2:**_ In this part the user needs to connect the Raspberry Pi via SSH then update the OS.

   - **Type SSH in the cmd to access the network protocol. Then type the following command:**
  > 1. **_ssh username@hostname (e.g. group12@group12)_**
  > 2. **_sudo apt update_**
  > 3. **_sudo apt upgrade_**

![403416157_334051386075788_6688766810160006595_n](https://github.com/CaseinBrt/Documentation/assets/145450481/1fa7a8d7-f065-45a4-8fed-6943a3296752)

 ---
 
 ![393192245_1031425994761262_4206474068423483197_n](https://github.com/CaseinBrt/Documentation/assets/145450481/6c92c8f1-a8c6-45da-bcc0-0ba0bb8043ac)
 
 ---
 
### _**Step 3:**_ Now, Install LAMP Stack. LAMP stands for **_Linux, Apache, MySQL, and PHP._**

> **_Here are the tutorials on how to install LAMP stack_** [[1]](https://ostechnix.com/install-apache-mysql-php-lamp-stack-on-ubuntu-18-04-lts/)[[2]](https://linuxhint.com/install-phpmyadmin-raspberry-pi/)

 - To install the stack, type the following commands on our command prompt connected to Raspberry Pia via SSH.
   
   >1. **_Sudo apt install apache2_**

   ![400593480_308372015496794_2291834078334473568_n](https://github.com/CaseinBrt/Documentation/assets/145450481/b0f4b10f-59a3-4f02-9df7-baaf7035232c)
  
   ---
     
   >2. **_sudo apt install mariadb-server_**

   ![403401528_3536484756591237_4185986630700900526_n](https://github.com/CaseinBrt/Documentation/assets/145450481/9ab89acf-1093-4149-8033-5205d8945ed8)

     ---
     
   >3. **_sudo mysql_secure_installation_**

     ![370207241_912270033664555_4978805515279109701_n](https://github.com/CaseinBrt/Documentation/assets/145450481/97736833-4dc5-4b84-a24f-024f45e9c461)

     ---
     
   >4. **_sudo apt install php libapache2-mod-php php-mysql_**

    ![367359434_725970812417267_9108233154384373995_n](https://github.com/CaseinBrt/Documentation/assets/145450481/d55225d4-43d9-4d22-92e4-9f3a3dc4372d)

     ---
     
   >5. **_sudo apt-get install php_**

    ![403403518_677772637671758_5130286334291612518_n](https://github.com/CaseinBrt/Documentation/assets/145450481/975fc2b5-bce1-4d23-8555-60efaf2d287e)

     ---
     
   >6. **_sudo apt install phpmyadmin_**

    ![400758392_1721342348342280_5591834237161218208_n](https://github.com/CaseinBrt/Documentation/assets/145450481/01861509-ffa3-45de-81da-49ce0af39194)

     ---

### _**Step 4:**_ Connect to **_Raspberry Pi via VNC_**
 + Install RealVNC® Viewer.
 + Before opening VNC on our chosen device, first thing we need to do is to enable VNC on the OS via the **_sudo raspi-config_** command into Raspberry Pi Configuration Tool
 + Navigate **"Interfacing Options"** >  **"VNC"**, Using the arrows, then choose **_"Yes"_** and select **_"OK"_**
   ---

    ![368033655_1418038518789351_3463345382618325401_n](https://github.com/CaseinBrt/Documentation/assets/145450481/4af998ad-f811-4419-adf5-0d2f4eb4ac9e)

   ---
   
    ![372318563_3528511977430546_4739800732196631453_n](https://github.com/CaseinBrt/Documentation/assets/145450481/da9db631-279c-44c0-8ef4-eca239f72301)

   ---

   ![401177787_1085340499142779_5373566576894757585_n](https://github.com/CaseinBrt/Documentation/assets/145450481/93372659-9e1a-45a1-8b69-13f8eba8e3ef)

   ---
   
    ![371533130_1424334041484770_378061606160522842_n](https://github.com/CaseinBrt/Documentation/assets/145450481/57f2bc8b-df92-4b63-a0b8-3184b3fa7932)

   ---
   
-  In this part we must take control on the device and run RealVNC Viewer... Enter the _private IP address_ in the search bar. If the screen of the Raspberry Pi appeared on **RealVNC**, it means that it established already the connection and control on the **_Raspberry Pi_**.

  ---
  
  ![393161962_351181004269522_416777685802602515_n](https://github.com/CaseinBrt/Documentation/assets/145450481/e2fb159e-35ed-4e5e-a1ce-800f7b309d28)








