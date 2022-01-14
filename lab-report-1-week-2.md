# Lab report

## Installing VScode

* Go to [VS Code Official Site](https://code.visualstudio.com)
* Click on the blue download button at the top right
![Image](ssForLab.PNG)
* This will lead you to the dowload page, choose you OS.
* Double click the .exe file.

## Remotely Connecting 
---
**Installing OpenSSH**
* You can do so by following the [guide](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse) along.
* Start by checking if OpenSSH is already installed
* Open Powershell as the administrator and run the following command:

* <span style="color:red"> *whole file fixed*</span>

```
Get-WindowsCapability -Online | Where-Object Name -like 'OpenSSH*'
```

* If it is not installed, this should be the output:

```
Name  : OpenSSH.Client~~~~0.0.1.0
State : NotPresent

Name  : OpenSSH.Server~~~~0.0.1.0
State : NotPresent
```

* Run the followings commands to download the Client or Server depending on which one was not present

```
# Install the OpenSSH Client
Add-WindowsCapability -Online -Name OpenSSH.Client~~~~0.0.1.0

# Install the OpenSSH Server
Add-WindowsCapability -Online -Name OpenSSH.Server~~~~0.0.1.0
```

* After this, the first command should output this:

```
Name  : OpenSSH.Client~~~~0.0.1.0
State : Installed

Name  : OpenSSH.Server~~~~0.0.1.0
State : Installed
```

---
**Finding your course specific account**
* Got to https://sdacs.ucsd.edu/~icc/index.php
* The page should look like this, input your username and  Student ID
![Image](ssForLab2.PNG)
* Here you can find your username and set your password. For this class it will look something like this: cs15lwi22***@ieng6.ucsd.edu
* The stars will be your own custom letters.

---
**Connecting**
* Open Visual Studio and hover over Terminal and click New Terminal
* Paste the following command but replacing the stars with your own letters.

```
$ ssh cs15lwi22***@ieng6.ucsd.edu
```

* As it is the first time logging in you will receive the following message. Just type yes then hit enter.

```
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])? 
```

* It will then ask you for your password, type in the one you got above. You will not see it appear as you type.

``` 
Password: 
Last login: Sun Jan  2 14:03:05 2022 from 107-217-10-235.lightspeed.sndgca.sbcglobal.net
quota: No filesystem specified.
Hello cs15lwi22zz, you are currently logged into ieng6-203.ucsd.edu

You are using 0% CPU on this system

Cluster Status 
Hostname     Time    #Users  Load  Averages  
ieng6-201   23:25:01   0  0.08,  0.17,  0.11
ieng6-202   23:25:01   1  0.09,  0.15,  0.11
ieng6-203   23:25:01   1  0.08,  0.15,  0.11

Sun Jan 02, 2022 11:28pm - Prepping cs15lwi22
```

* You are connected!

---

## Trying Some Commands

Now to run some commands locally and remotely:
* pwd (prints work directory)
* mkdir (makes a new directory)
* cp (copy)
* cd ~ (brings you back to home path)
* cd (change directory)
* ls (prints what is inside the directory)
* ls -lat
* ls -a (prints everything what is inside the directory)
* cat

**Example:**
![Image](ssForLab3.PNG)


## Moving Files with scp
## Setting an SSH Key
## Optimizing Remote Running
