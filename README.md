# CONFIGURATION OF SOURCETREE WITH SSH KEY FROM GITHUB

(FOR READING THIS ARTICLE IN A FRIENDLY WAY YOU SHOULD DO THIS)

```shell
clone this repository to your computer and then inside readme page, you should use this command

open up with VSCODE

ctrl + shift + v

```

## GENERATING AN SSH IN GitHub:

1- Follow the steps to set up SSH authentication for github https://docs.github.com/en/authentication/connecting-to-github-with-ssh

## VINCULATION WITH SOURCETREE:

2 - Open up ST

- 2.1 - Skip to Bitbucket option.

- 2.2 - Do not mark the checkbox 'mercurial', Next.

  ![](./img/7.png)

- 2.3 - Add a user name and an email from your company, next.

  ![](./img/8.png)

* 2.4 - The following popup will appear, and select 'no'

  ![](./img/9.png)

## WORKING WITH SOURCETREE

3 - Go to the repository needed to clone and copy the SSH route.

![](./img/10.png)

- 3.1 - Again in ST, option 'clone'

  ![](./img/11.png)

- 3.2 - Paste de SSH route from the repository in the fill like the image and hit enter.

  ![](./img/12.png)

- 3.3 - The following popup will appear, and select 'Yes'.

  ![](./img/13.png)

- 3.4 - Select NO when asked about loading a SSH key. Source tree uses Putty auth agent for managing the private keys and needs them to be converted to a different format before loading them (instructions in the next section).

  ![](./img/14.png)

## Putty

4 - Putty allows us to convert SSH keys to the format it supports. Inside ST we access in this way.

- 4.1 - In ST searchbar: Tools / Create or Import.

  ![](./img/16.png)

- 4.2 - The following popup will appear, and select 'Load'.

  ![](./img/17.png)

- 4.3 - The program will look for a .ppk file and we don't have it yet. For that reason we must select 'All files' so that we can list all the available files.

  ![](./img/21.png)

- 4.4 - Choose your SSH key and touch 'Open'

  ![](./img/22.png)

- 4.5 - This will automatically make a process of converting our key to .ppk. The following popup will appear, and select 'Accept'.

  ![](./img/23.png)

- 4.6 - Now touch 'Save private key' We are going to be asked if we want to activate the key without a passphrase, We choose 'Yes'.

  ![](./img/24.png)
  ![](./img/25.png)

- 4.7 -The route where our keys are will be open again, but this time, We need to choose a name and next in 'Save' The SSH was converted to .ppk, but we still need to connect our project.

  ![](./img/26.png)

## CONNECTING THE PROJECT WITH SSH KEY .ppk

5 - We should open Putty for authentication. You can see where the program is, in the image.

![](./img/28.png)

- 5.1 - After this We are allowed to put our SSH .ppk created before. Press 'Add key'.

  ![](./img/27.png)

- 5.2 - The following folder will appear, and we need to select the .ppk SSH created, in my case, this is 'perp.ppk'

  ![](./img/29.png)

- 5.3 - This will load our private key into putty authentication agent.

## CLONING THE PROJECT

6 - Go back to ST, again with SSH code from the project.

- 6.1 - Press option 'clone'
  ![](./img/11.png)

- 6.2 - Paste the copied code from GitHub inside the shown field and hit enter on your keyboard.

  ![](./img/12.png)

- 6.1 - Choose a destiny folder for the project and name it. Press 'Advanced options' and inside this press 'Checkout branch' and choose 'Develop' like in the image.

  ![](./img/31.png)

- 6.3 - check 'Recurse submodules' must be chosen.

  ![](./img/32.png)

- 6.4 - Hit 'Clone'. After that, We should be allowed to work with the project.

  ![](./img/34.png)
## INSIDE THE PROJECT
