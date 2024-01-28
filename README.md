# OSProject Running Containers for Application Development

Group Name: OS

Section: 2 

Team Mates:
1. Mamun Mekdam Bin 2122727
2. FARHAN AKBAR CHOWDHURY 2028705


## Rules
1. You are allowed to have **3 group** members. *Exception* is allowed **IFF (if and only if)** you are allowed to have 4 group members if you are a **multinational** or a **multigender** group. 
2. When you complete the project, make sure to submit the repository link of your cloned project. Make sure all the files are as what you aspect in your repository. 
3. Answer all questions in the **README.md**, in your own repository. Either use the online VSCode, terminal or github to edit. Answers are expected where you see __Fill answer here__.
4. Learn how to use markdown. https://www.w3schools.io/file/markdown-introduction/

## Forking this OS project repository
1. First thing you need in doing this project is to have a github account. Make sure to sign up at https://www.github.com
2. The second thing you need is to fork the OS project repository in your own github account. 

    1. Go to https://github.com/joeynor/OSProject and click fork to copy the project into your own repository
    2. Make sure that the new fork is now in your own repository

***Questions:***

1. What is the link of the fork OSProject in your repository. ***(1 mark)*** __https://github.com/MekdamMamun/OSProject__.
2. How many files and folders are in this repository. ***(1 mark)*** __Fill answer here__.


## Exploring github codespaces

1. The next thing that we will be doing is exploring codespaces. First of all, read about codespaces https://docs.github.com/en/codespaces/overview#what-is-a-codespace
2. Then go to the link https://github.com/codespaces and we shall start a new codespace.  
3. Click on ***New codespace***.
4. Choose your own OSProject repository to start your codespace.

 <img src="./images/newcodespace.png" width="50%">

5. Once you have created you codespace, you will see the following. You might already be familiar with this, since it will look similar to VSCode. 

 <img src="./images/UIwebvscode.png" width="70%">

6. You will see the [README file](./README.md) file. One is a preview of how it looks like on the web, and the other is the editing view in markdown language. 
7. Edit the [README file](./README.md). Make sure you have your group details correct, ie, group name, section and team members along with their matric IDs. 
8. Once you have finish editing, click File->Save or ***ctrl-s*** to save it. 
9. After saving, you will notice an M or U next to your file. You will need to commit any changes, whenever you make changes so that it is uploaded to the github repository. 

 <img src="./images/SourceControlUI.png" width="70%">

10. Click on the source control, hint: its on the left side panel, and it will list down the files that have been modified or updated. Click on commit. It will then ask you "Would you like to stage all your changes and commit them directly?" Just say yes, and a new tab will appear. Type a message to log what you have done, and click on the check mark. 

 <img src="./images/CommittingUI.png" width="70%">

11. After that, sync the changes to the main repository. 
12. Make sure to commit and sync your files to the main repository, or else, your work will be lost since it is not saved into the main repository when you submit your project.

***Questions:***

1. What is default OS used to run the virtual environment for codespaces. ***(1 mark)*** __Ubuntu Linux__.
2. What are the two options of ram, disk and vcpu configuration you can have in running codespaces . ***(1 mark)***
    __Standard Configuration:
RAM: 4 GB
Disk Space: 32 GB
vCPU: 1 core
Enhanced Configuration:
RAM: 8 GB
Disk Space: 64 GB
vCPU: 2 cores__.
4. Why must we commit and sync our current work on source control? ***(1 mark)***
   __Preserves Changes: Captures a snapshot of your current work, preserving changes and allowing you to revert if needed.
Collaboration: Enables collaboration by sharing updates with team members, ensuring everyone has access to the latest code.
Backup: Serves as a backup, protecting your work from accidental loss or system failures.__.

## Exploring the Terminal

1. Look at the TERMINAL tab. Explore and run commands according to the questions below. 
2. You can include your answers as images, or cut and paste the output here. If you are cutting and pasting your answers, wrap your answers in the codeblock clause in markdown. For example, if i run the command **whoami** the the output would look like the one below.
```bash
@joeynor ➜ /workspaces/OSProject (main) $ whoami 
codespace
```



***Questions:***

Look at the TERMINAL tab. Run the following commands and provide the output here. 

1. Run the command **pwd** . ***(1 mark)*** __![Alt text](Os 1.png)__.
2. Run the command **cat /etc/passwd** . ***(1 mark)*** __![Alt text](Os 2.png)__.
3. Run the command **df** . ***(1 mark)*** __![Alt text](OS 3.png)__.
4. Run the command **du** . ***(1 mark)*** __![Alt text](OS 4.1.png) / ![Alt text](OS 4.2.png)__.
5. Run the command **ls** . ***(1 mark)*** __![Alt text](OS 5.png)__.
6. Run the command **ls -asl** . ***(1 mark)*** __![Alt text](OS 6.png)__.
7. Run the command **free -h** . ***(1 mark)*** __![Alt text](OS 7.png)__.
8. Run the command **cat /proc/cpuinfo** . ***(1 mark)*** __![Alt text](OS 8.png)__.
9. Run the command **top** and type **q** to quit. ***(1 mark)*** __![Alt text](OS 9.png)__.
10. Run the command **uname -a**. ***(1 mark)*** __![Alt text](OS 10.png)__.
11. What is the available free memory in the system. ***(1 mark)*** __237Mi__.
12. What is the available disk space mounted on /workspace. ***(1 mark)*** __5Gi__.
13. Name the version and hardware architecture of the linux Virtual environment. ***(1 mark)*** __Linux codespaces-10daca 6.2.0-1018-azure #18-22.04.1-Ubuntu SMP Tue Nov 21 19:25:02 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux__.
14. What is the difference between **ls** vs **ls -asl**. ***(1 mark)***
__ls' is the basic command that simply lists the name of the files and directories meanwhile 'ls -asl' is a customized option command that provides a more detailed listing, such as hidden files, sizes in blocks, and additional information about each file__.
16. What is the TLB size of the Virtual CPU. ***(1 mark)*** __2560 4K pages__.
17. What is the CPU speed of the Virtual CPU. ***(1 mark)*** __2877.951MHz__.
18. What is the top running process that consumes the most CPU cycles. ***(1 mark)*** __14:32:54 up 49 min,  0 users,  load average: 0.03, 0.16, 0.35__.

## Running your own container instance.

1. At the terminal, run a linux instance. By typing the following command. 
```
docker pull debian
docker run --detach -it debian
```
2. This will run the debian container. To check if the debian container is running, type
```bash
@joeynor ➜ /workspaces/OSProject (main) $ docker ps -a
CONTAINER ID   IMAGE     COMMAND   CREATED         STATUS         PORTS     NAMES
f65be1987f84   debian    "bash"    4 minutes ago   Up 4 minutes             romantic_jackson
```

3. Keep note of the name used by your container, this is usually given random names unless you specify your own name. Now run a bash command on the container. Make sure you use the name of your container instead of the one shown here. 
```bash
docker exec -i -t romantic_jackson /bin/bash
```

4. Create a file on the container. First you must make sure you are in the bash command prompt of the container. The container is new, and does not have any software other than the debian OS. To create a new file, you will need an editor installed. In the bash shell of the container, run the package manager apt-get to install nano text editor. 

```bash
root@f65be1987f84:~# apt-get update      

root@f65be1987f84:~# apt-get install nano

root@f65be1987f84:~# cd /root

root@f65be1987f84:~# nano helloworld.txt
```

5. Edit your helloworld.txt, create your messsage and save by typing ctrl-X. Once saved, explore using the container to see where the file is located. Then exit the shell, by typing **exit**.

6. Stop the container and run **docker ps -a**, and restart the container again. Is your file in the container still available?
```bash 
@joeynor ➜ /workspaces/OSProject (main) $ docker stop romantic_jackson

@joeynor ➜ /workspaces/OSProject (main) $ docker ps -a
CONTAINER ID   IMAGE     COMMAND   CREATED          STATUS                        PORTS     NAMES
f65be1987f84   debian    "bash"    19 minutes ago   Exited (137) 18 seconds ago             romantic_jackson

@joeynor ➜ /workspaces/OSProject (main) $ docker restart romantic_jackson
```

7. Stop the container and delete the container. What happened to your helloworld.txt?

```bash 
@joeynor ➜ /workspaces/OSProject (main) $ docker stop romantic_jackson

@joeynor ➜ /workspaces/OSProject (main) $ docker ps -a
CONTAINER ID   IMAGE     COMMAND   CREATED          STATUS                        PORTS     NAMES
f65be1987f84   debian    "bash"    19 minutes ago   Exited (137) 18 seconds ago             romantic_jackson

@joeynor ➜ /workspaces/OSProject (main) $ docker rm romantic_jackson
```

***Questions:***

1. Are files in the container persistent. Why not?. ***(1 mark)*** __Files in a container are typically not persistent by default because containers are designed to be stateless and ephemeral, prioritizing scalability and reproducibility over persistent storage.__.
2. Can we run two, or three instances of debian linux? . ***(1 mark)*** __Yes__.

## Running your own container with persistent storage

1. In the previous experiment, you might have notice that containers are not persistent. To make storage persistent, you will need to mount them. 
At the terminal, create a new directory called **myroot**, and run a instance of debian linux and mount myroot to the container. Find out the exact path of my root, and mount it as the root folder in the debian container. 
2. Create a file in /root on the container, the files should also appear in myroot of your host VM.

```bash 
@joeynor ➜ /workspaces/OSProject (main) $ mkdir myroot
@joeynor ➜ /workspaces/OSProject (main) $ cd myroot/
@joeynor ➜ /workspaces/OSProject/myroot (main) $ pwd
/workspaces/OSProject/myroot

@joeynor ➜ /workspaces/OSProject/myroot (main) $ docker run --detach -it -v /workspaces/OSProject/myroot:/root debian
```

***Questions:***

1. Check the permission of the files created in myroot, what user and group is the files created in docker container on the host virtual machine? . ***(2 mark)*** __total 32
 4 drwxrwxrwx+ 5 codespace root  4096 Jan 28 14:15  .
 4 drwxr-xrwx+ 5 codespace root  4096 Jan 28 14:15  ..
 4 drwxrwxrwx+ 9 codespace root  4096 Jan 28 14:16  .git
 4 drwxrwxrwx+ 2 codespace root  4096 Jan 28 14:15 'GROUP project'
12 -rw-rw-rw-  1 codespace root 11343 Jan 28 14:15  README.md
 4 drwxrwxrwx+ 2 codespace root  4096 Jan 28 14:15  images__.
2. Can you change the permission of the files to user codespace.  You will need this to be able to commit and get points for this question. ***(2 mark)***
```bash
//use sudo and chown
sudo chown -R codespace:codespace myroot

```
*** __ 4 drwxr-xrwx+ 5 codespace root  4096 Jan 28 14:15__.***

## You are on your own, create your own static webpage

1. Create a directory called webpage in your host machine
2. Inside the directory, create a page index.html, with any content you would like
3. Then, run the apache webserver and mount the webpage directory to it. Hint:
```bash
## the -p 8080:80 flag points the host port 8080 to the container port 80

docker run --detach -v /workspaces/OSProject/webpage:/usr/local/apache2/htdocs/ -p 8080:80 httpd
```

4. If it works, codespace will trigger a port assignment and provide a URL for you to access your webpage like the one below.

 <img src="./images/websitelink.png" width="70%">


5. You can also see the Port in the **PORTS** tab, next to the terminal tab.

6. You can then access your website by adding an index.html towards the end of your url link, like the one below. 

 <img src="./images/helloworldweb.png" width="70%">

***Questions:***

1. What is the permission of folder /usr/local/apache/htdocs and what user and group owns the folder? . ***(2 mark)*** __ 4 drwxrwxrwx+ 2 codespace root  4096 Jan 28 14:15/usr/local/apache/htdocs__.
2. What port is the apache web server running. ***(1 mark)*** =8080
3. What port is open for http protocol on the host machine? ***(1 mark)***="80"

## What to submit

1. Make sure to commit all changes on your source control, and make sure your source control is sync to the repository. 
2. Check your repository link, to see if all the files and answers are included in the repository. 
3. Submit through italeem, by providing the link to your repository.
4. Due by ***31 January, 2024***
