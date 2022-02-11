 <font size="12"> Lab Report 3 Week 6</font>
 
# Streamlining ssh Configuration

## Show your .ssh/config file, and how you edited it (with VScode, another program, etc)

![Image](ssLab1.PNG)

Access the .ssh folder which is in your home. Type: **notepad config**. To create the file and open it in a notepad. Copy the text below and replace zzz with your id.

```
Host ieng6
    HostName ieng6.ucsd.edu
    User cs15lwi22zzz
    IdentityFile ~/.ssh/id_rsa
```

## Show the ssh command logging you into your account using just the alias you chose.

![Image](ssLab2.PNG)

Now just by typing the command: **ssh ieng6** loggs into your remote acccess.

## Show an scp command copying a file to your account using just the alias you chose. 

![Image](ssLab3.PNG)

This now makes all commands requiring ssh much faster. Instead of having to type:

```
scp fileToMove.txt cs15lwi22anb@ieng6.ucsd.edu:~/
```

You can type:

```
scp fileToMove.txt ieng6:~/
```
