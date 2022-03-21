## AUX PROJECT 1: SHELL SCRIPTING

In this project, I created onboard 20 new Linux users onto a server. Created a shell script that reads a csv file that contains the first name of the users to be onboarded.

1. *Create the project folder called Shell*
   >mkdir Shell

     *Move into the Shell folder*

    >cd Shell

2. *Create a csv file name names.csv*

    >touch names.csv

    *Open the names.csv file*

     >vim names.csv

![](2022-03-21-22-46-10.png)

Note: Shell Script 

##### onboarding.sh
![](2022-03-21-22-43-50.png)
![](2022-03-21-22-45-32.png)

A. After I created the script to read the CSV file:

B. Each user on the server, added to an existing group called developers.

![](2022-03-21-22-47-15.png)

C. I Ensure that the script will first check for the existence of the user on the system, before it will attempt to create that it.

![](2022-03-21-22-48-04.png)

D. I Ensure that the user that is being created also has a default home folder.

E. I Ensure that each user has a .ssh folder within its HOME folder.

F. For each user’s, the SSH configuration, I created an authorized_keys file and add ensxure it has the public key for the current user.

![](2022-03-21-22-48-54.png)


Before Deploying my script, I updated the current user with the correct public key and private key.

Home directory .ssh folder

> cd .ssh

create a file for the public key

> touch id_rsa.pub

open the file using your favorite editor and paste in the public key

> vi id_rsa.pub

create a file for your private key

> touch id_rsa

open the file using your favorite editor and paste in the private key.

![](2022-03-21-23-56-48.png)

> vi id_rsa

The Public Key

![](2022-03-21-23-57-16.png)




Note:

## Test a few of the users randomly, and ensure that you are able to connect to the server using the private key and the public key.

### USER - Olu

Test a few of the users randomly, and ensure that you are able to connect to the server using the private key and the public key.

![](2022-03-21-22-51-26.png)

### USER Biola

![](2022-03-21-22-53-01.png)

### USER Bright

![](2022-03-21-22-53-40.png)


