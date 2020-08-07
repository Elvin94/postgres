# How to install postgres database server on LinuxONE Community Cloud
Open source software is increasingly becoming available on the mainframe(IBM z/LinuxONE). PostgreSQL, also known as Postgres, is a free and open-source relational database management system emphasizing extensibility and SQL compliance. 

There are benefits running Postgres, the features is aimed to help developers build applications, administrators to protect data integrity and build fault-tolerant environments, and help you manage data no matter how big or small the dataset.
In this tutorial, we’ll be using Rhel 8 and Sles 15, which are popular Linux Platform compatible to LinuxONE machine. Some steps might be little different if you are using different architecture

## Register for LinuxONE Community Cloud
1) In a browser, go to the [LinuxONE Community Cloud website](https://ibm.biz/linuxonecc).
2) Click **Try a Virtual Machines on the LinuxONE Community Cloud** now.
3) Complete the required fields on the registration form.
4) Complete your registration by clicking **Request your trial**.
5) Check your email for a registration confirmation similar to the following shown. You will need your User ID and Password from this email to sign in to the self service portal

## VM Setup

1) After activating your account, log in.

* Enter your **user ID** and the **password** created during registration.
* Click **Sign in**.

2) Now is also a good time to create or import an SSH key. An SSH public key is required to deploy Linux instance. The instance can only be accessed with your private key that matches the public key.
* Click your **username** from the upper right corner of the Home page.
* Select **Manage SSH Key Pairs**.

3) If you already have a public SSH key you wish to use with this cloud:    
   * Click **Import**. 
   * Enter a **Key Name** for this key.
   * Browse your local file system to select the **public key path**.
   * Click **Upload your public key**.

4) If you want to create a new SSH key pair:     
* Click **Create**.
* Enter a **Key Name** for this key.
* Click **Create a new key pair**.   
* A pop-up window will appear asking you to save **yourkey. pem** file. This is your private key.  Please save it to a secure location.  Once this operation is complete, there is no way to retrieve this key. Click **OK** to save the file. 

