# How to install postgres database server on LinuxONE Community Cloud
Open source software is increasingly becoming available on the mainframe(IBM z/LinuxONE). PostgreSQL, also known as Postgres, is a free and open-source relational database management system emphasizing extensibility and SQL compliance. 

There are benefits running Postgres, the features is aimed to help developers build applications, administrators to protect data integrity and build fault-tolerant environments, and help you manage data no matter how big or small the dataset.
In this tutorial, we’ll be using Rhel 8 and Sles 15, which are popular Linux Platform compatible to LinuxONE machine. Some steps might be little different if you are using different architecture

## Prerequisites
 1. Request access to LinuxONE Community Cloud. Follow instructions [here](https://github.com/Elvin94/LinuxONE-OSS-CC)


### Step 1: Install postgres database server on LinuxONE Community Cloud
   1. Import postgres package
   ```sh
   rpm --import http://packages.2ndquadrant.com/postgresql-z/RPM-GPG-KEY-2NDQ-RHEL7
    ```
   2. Configure yum repo



# How to install postgres database server on LinuxONE Community Cloud


rpm --import http://packages.2ndquadrant.com/postgresql-z/RPM-GPG-KEY-2NDQ-RHEL7

3) Firewall is enabled. Only the SSH port is open.  Modify the firewall rules with iptables if you need other ports opened. For example:
   ```sh
   iptables -I INPUT -p tcp --dport <port#> -j ACCEPT 
   ```
   If you want to make your changes permanently, issue this command:
   ```sh
   iptables-save > /etc/sysconfig/iptables 
   ```
## Important notes about your server:
1) You can use ‘sudo’ to execute commands that require root authority.

2) It could take up to 10 minutes to format and mount the /data disk.  Issue the following command to verify the /data disk is available before continuing:
   ```sh
   df -h 
   ```
   ![alt text](images/create_schema.png "Check /data disk")
