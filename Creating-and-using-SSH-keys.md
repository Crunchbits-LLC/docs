# Creating and using SSH keys

1.  On the left top, click SSH Keys

![1241235423523524.png](Creating%20and%20using%20SSH%20keys%20%5BVF%20Only%5D%20a0b8b87d548c46c0803fea77b5f146b7/1241235423523524.png)

2. Click Add Key

![KBSSHKETS.png](Creating%20and%20using%20SSH%20keys%20%5BVF%20Only%5D%20a0b8b87d548c46c0803fea77b5f146b7/KBSSHKETS.png)

3. Add a name to the key and click Generate Key Pair

![Bez nazwy.png](Creating%20and%20using%20SSH%20keys%20%5BVF%20Only%5D%20a0b8b87d548c46c0803fea77b5f146b7/Bez_nazwy.png)

4. Leave all the options default, and click Generate 

![noname2.png](Creating%20and%20using%20SSH%20keys%20%5BVF%20Only%5D%20a0b8b87d548c46c0803fea77b5f146b7/noname2.png)

5. Copy the private key to your computer. 
6. Copy the public key to your computer with the extension .pub

![nononame.png](Creating%20and%20using%20SSH%20keys%20%5BVF%20Only%5D%20a0b8b87d548c46c0803fea77b5f146b7/nononame.png)

7. Click Save

![123123123.png](Creating%20and%20using%20SSH%20keys%20%5BVF%20Only%5D%20a0b8b87d548c46c0803fea77b5f146b7/123123123.png)

### How to generate SSH keys on Ubuntu/Debian

Here's a step-by-step guide on how to generate and add SSH keys to Ubuntu or Debian:

1. Open a terminal on your Ubuntu/Debian machine (NOT THE SERVER! We are generating your key pair so this has to be done on your local system) and type the following command:

<code>ssh-keygen -t rsa</code>
This will start the ssh-keygen utility, which will prompt you to specify a location to save the key. By default, the utility will save the key in the ~/.ssh/ directory with the filename id_rsa. You can accept the default location by pressing Enter.
 
The utility will then prompt you to enter a passphrase. This is an optional security measure that adds an additional layer of protection to your SSH key. If you choose to set a passphrase, you will be required to enter it each time you use the key. If you prefer not to set a passphrase, just pressEnter.

2. Once the key has been generated, you can view it by running the following command:

<code>cat ~/.ssh/id_rsa.pub</code>
This will print the contents of your public SSH key to the terminal.

3. To add the key to your account on a remote server, you will need to copy the contents of your public key and add it to the ~/.ssh/authorized_keys file on the remote server. You can do this by running the following command while logged in via ssh on the remote server:

<code>echo "paste-your-key-here" >> ~/.ssh/authorized_keys</code>
Replace "paste-your-key-here" with the contents of your public SSH key. Make sure to include the entire key, including the <code>ssh-rsa</code> at the beginning and the username@hostname at the end.

### How to generate SSH keys on Windows

Here's a step-by-step guide on how to generate SSH keys in Windows:

1. Download and install the latest version of PuTTY, which is a free SSH client for Windows. You can download PuTTY from the following link:

https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html

2. Once PuTTY is installed, open the PuTTYgen utility, which is a tool for generating SSH keys. You can do this by searching for "PuTTYgen" in the Start menu.

3. In the "Type of key to generate" field, select "SSH-2 RSA" and click the "Generate" button.

4. PuTTYgen will then prompt you to move your mouse around in the blank area below the progress bar. This is to generate some randomness, which is used to create your SSH key.

5. Once the key has been generated, PuTTYgen will display the public and private parts of the key. The public key is the one that you will need to add to the remote server, while the private key is the one that you will use to authenticate yourself when connecting to the server.

6. To save the public key, click the "Save public key" button and specify a location to save the file. Make sure to save the file with a <code>.pub</code> extension, such as <code>my_key.pub</code>.

7. To save the private key, click the "Save private key" button and specify a location to save the file. Make sure to save the file with a <code>.ppk</code> extension, such as <code>my_key.ppk</code>.

8. To add the public key to your account on the remote server, you will need to copy the contents of the <code>.pub</code> file and add it to the <code>~/.ssh/authorized_keys</code> file on the remote server. You can do this using a tool such as WinSCP or via ssh.

### How to add your public SSH key to an existing Ubuntu/Debian server

To add your public SSH key to a remote Ubuntu or Debian server, follow these steps:

1. Copy your public SSH key to your clipboard.

2. Connect to the remote Ubuntu server using SSH. Note that whatever user you connect as is also going to be the same as the account which we are adding the SSH keys.

3. Once you are connected to the server, create a .ssh directory in your home directory if it doesn't already exist:

<code>mkdir ~/.ssh</code>

4. Open the authorized_keys file in a text editor, such as nano:

<code>nano ~/.ssh/authorized_keys</code>

5. Paste your public SSH key into the authorized_keys file. You can do this by right-clicking in the terminal window and selecting "Paste" from the context menu, or by using the paste command in nano: Ctrl+Shift+V
6. Save the authorized_keys file and exit the text editor.
7. Set the correct permissions on the .ssh directory and authorized_keys file:

<code>chmod 700 ~/.ssh</code>
<code>chmod 600 ~/.ssh/authorized_keys</code>

### Using SSH Keys:

<code>ssh -i /path/to/privatekey root@crucnhbits.com</code>
