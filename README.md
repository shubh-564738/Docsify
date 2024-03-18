# Docsify

<br>
<br>

**Table of content**


* [What is Docsify](#What-is-Docsify)
* [Features](#Features)
* Installation
* Initialised
<br>
<br>

# What is Docsify?

Docsify is an open-source, simple, and lightweight documentation generator that utilizes Markdown files to create customizable websites. It is ideal for technical documentation, project wikis, and knowledge bases.

<br>
<br>

# Features

* No statically built html files
* Simple and lightweight
* Smart full-text search plugin
* Multiple themes
* Useful plugin API
* Emoji support
* Compatible with IE11
* Support server-side rendering

<br>
<br>
  
**Installation**

<br>

**Step1-** 
you have to install some important dependencies to run Docsify.
```
sudo apt update
```
**output-**

~~~
shubham@shubham-Latitude-7480:~$ sudo apt update
[sudo] password for shubham: 
Hit:2 https://dl.google.com/linux/chrome/deb stable InRelease                  
Hit:1 https://packages.microsoft.com/repos/code stable InRelease               
Hit:3 http://in.archive.ubuntu.com/ubuntu jammy InRelease                      
Get:4 http://security.ubuntu.com/ubuntu jammy-security InRelease [110 kB]      
Get:5 http://in.archive.ubuntu.com/ubuntu jammy-updates InRelease [119 kB]
Hit:6 http://in.archive.ubuntu.com/ubuntu jammy-backports InRelease 
Fetched 229 kB in 3s (66.9 kB/s)
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
155 packages can be upgraded. Run 'apt list --upgradable' to see them.
~~~

<br>

**sudo:** Gives you special permission to do important stuff.

**apt:** The tool that manages software on your computer.

**update:** Tells the software tool to check for new stuff to install or update.

<br>
<br>
<br>

**Step2-**
1) First, check if Node.js and npm are installed on your machine.

2) To check if Node.js is installed, type the following command 
```
node -v
```
This command will display the installed Node.js version if it is installed. If Node.js is not installed, you will see an error message.

<br>

**node:** Refers to the Node.js runtime environment.

**-v:** Stands for version.

<br>
<br>
<br>

 3) To check if npm is installed, type the following command
    
```
npm -v
```
This command will display the installed npm version if it is installed. If npm is not installed, you will see an error message.

<br>

**npm:** Stands for Node Package Manager, used to manage packages and dependencies in Node.js projects.

**-v:** Stands for Version.

<br>
<br>
<br>

4) If you haven't installed Node.js and npm yet, you can do so by following these steps

```bash
sudo apt install nodejs npm
```
**output-**

~~~
shubham@shubham-Latitude-7480:~$ sudo apt install nodejs npm
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
npm is already the newest version (8.5.1~ds-1).
The following additional packages will be installed:
  libnode-dev libnode72
The following packages will be upgraded:
  libnode-dev libnode72 nodejs
3 upgraded, 0 newly installed, 0 to remove and 152 not upgraded.
Need to get 11.5 MB of archives.
After this operation, 4,096 B of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 http://in.archive.ubuntu.com/ubuntu jammy-updates/universe amd64 nodejs amd64 12.22.9~dfsg-1ubuntu3.4 [122 kB]
Get:2 http://in.archive.ubuntu.com/ubuntu jammy-updates/universe amd64 libnode-dev amd64 12.22.9~dfsg-1ubuntu3.4 [609 kB]
Get:3 http://in.archive.ubuntu.com/ubuntu jammy-updates/universe amd64 libnode72 amd64 12.22.9~dfsg-1ubuntu3.4 [10.8 MB]
Fetched 11.5 MB in 8s (1,430 kB/s)                                             
(Reading database ... 234113 files and directories currently installed.)
Preparing to unpack .../nodejs_12.22.9~dfsg-1ubuntu3.4_amd64.deb ...
Unpacking nodejs (12.22.9~dfsg-1ubuntu3.4) over (12.22.9~dfsg-1ubuntu3.3) ...
Preparing to unpack .../libnode-dev_12.22.9~dfsg-1ubuntu3.4_amd64.deb ...
Unpacking libnode-dev (12.22.9~dfsg-1ubuntu3.4) over (12.22.9~dfsg-1ubuntu3.3) .
..
Preparing to unpack .../libnode72_12.22.9~dfsg-1ubuntu3.4_amd64.deb ...
Unpacking libnode72:amd64 (12.22.9~dfsg-1ubuntu3.4) over (12.22.9~dfsg-1ubuntu3.
3) ...
Setting up libnode72:amd64 (12.22.9~dfsg-1ubuntu3.4) ...
Setting up libnode-dev (12.22.9~dfsg-1ubuntu3.4) ...
Setting up nodejs (12.22.9~dfsg-1ubuntu3.4) ...
Processing triggers for libc-bin (2.35-0ubuntu3.6) ...
Processing triggers for man-db (2.10.2-1) ...
~~~
<br>

**sudo:** Gives you special permission to install software, like Node.js and npm.

**apt:** The tool that manages software on your computer.

**install:** Tells apt to download and install the specified software packages.

**nodejs:** The name of the package for Node.js, which allows you to run JavaScript on your computer.

**npm:** Stands for Node Package Manager, used to manage JavaScript packages and dependencies.

<br>
<br>
<br>

**Step3-**
Once you have Node.js and npm installed, you can use npm to install Docsify using the following command

```bash
sudo npm install -g docsify-cli
```


**output-**
~~~
added 204 packages, and audited 205 packages in 18s

16 packages are looking for funding
  run `npm fund` for details

7 vulnerabilities (6 moderate, 1 high)

To address issues that do not require attention, run:
  npm audit fix

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.
~~~


**sudo:** Gives you special permission to install the package globally.

**npm:** Stands for Node Package Manager, used to manage JavaScript packages and dependencies.

**install:** Tells npm to download and install the specified package.

**-g:** Stands for "global," which means the package will be installed globally and accessible from anywhere in your system.

**docsify-cli:** The name of the package being installed, which is a command-line tool for generating and serving docsify documentation sites.

<br>
<br>
<br>

**Step4-**
After installation, you can verify that Docsify has been installed correctly by checking its version


```
docsify -v
```
**output-**
~~~
shubham@shubham-Latitude-7480:~$ docsify -v

docsify-cli version:
  4.4.4
~~~

**docsify:** Refers to the Docsify command-line tool.

**-version:** An option that tells the Docsify tool to display its version number.

<br>
<br>
<br>

**Initialised**


```bash
docsify init ./docs
```
**output-**
~~~
shubham@shubham-Latitude-7480:~$ docsify init ./docs
Initialization succeeded! Please run docsify serve ./docs
~~~

**docsify:** Refers to the Docsify command-line tool.

**init:** A command used to initialize or set up a new Docsify project.

**./docs:** Specifies the directory where the Docsify project will be initialized. 

<br>
<br>

If you want to preview your written content, run the below commands
```
docsify serve
```

It will run the local server as Docsify.

http://localhost:3000

**output-**

~~~
Serving /home/shubham/docs now.
Listening at http://localhost:3000
~~~

**docsify:** Refers to the Docsify command-line tool.

**serve:** This command tells Docsify to start a local development server to serve your documentation website.

<br>
<br>

**Congratulations! Now you have successfully installed Docsify.**










