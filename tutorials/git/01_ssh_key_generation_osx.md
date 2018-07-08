# How to generate SSH Key on Mac OS X

## Preface
SSH Key is way to access remote resources without entering login and password. It is like a lock (public key) that you put on remote resource and a key, that you always keep on your device (private key). Once you start using it, you will find it way more easy than using login and password all the time. 

You generate an SSH key through Mac OS X by using the Terminal application. Initially it looks like something hackers only can do, but there is nothing scary :). 


HELLO WORLD!!!!

## About the Terminal application

The terminal provides you with a text-based command line interface to the Unix shell of Mac OS X. 
You can think about it as an oldschool chatbot.

To open the Mac OS X Terminal, follow these steps:

1. In Finder, choose Utilities from the Go menu.
2. Find the Terminal application in the Utilities window.
3. Double-click the Terminal application.

The Terminal window opens with the command line prompt displaying the name of your machine and your username.

## Generating an SSH key

An SSH key consists of a pair of files. One is the private key, which you should never give to anyone nor send over internet even to yourself. The other is the public key. You will need a public key to access GOGs, virtual machines, and many other remote resources.

To generate SSH keys in Mac OS X, follow these steps:

1. Enter the following command in the Terminal window.
```
ssh-keygen -t rsa
```
This starts the key generation process. When you execute this command, the `ssh-keygen` utility prompts you to indicate where to store the key.

2. Press the ENTER key to accept the default location. The `ssh-keygen` utility prompts you for a passphrase.

Type in a passphrase. You can also hit the ENTER key to accept the default (no passphrase). However, this is not recommended.

**Warning!** You will need to enter the passphrase a second time to continue.

After you confirm the passphrase, the system generates the key pair.
```
Your identification has been saved in /Users/myname/.ssh/id_rsa.
Your public key has been saved in /Users/myname/.ssh/id_rsa.pub.
The key fingerprint is:
ae:89:72:0b:85:da:5a:f4:7c:1f:c2:43:fd:c6:44:38 myname@mymac.local
The key's randomart image is:
+--[ RSA 2048]----+
|                 |
|         .       |
|        E .      |
|   .   . o       |
|  o . . S .      |
| + + o . +       |
|. + o = o +      |
| o...o * o       |
|.  oo.o .        |
+-----------------+
```
Your private key is saved to the `id_rsa` file in the `.ssh` directory and is used to verify the public key (lock) you use put on remote resources corresponds to your private key (real key).

**Never share your private key with anyone!**
Your public key is saved to the `id_rsa.pub` file and is the key you can upload to remote resources or share with anyone you need. You can print this key to the screen by running following command:
```
cat ~/.ssh/id_rsa.pub
```           