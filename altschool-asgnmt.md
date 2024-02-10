<h1>ASSIGNMENT</h1>

`Question:` Your login name: altschool i.e home directory /home/ altschool. The home directory contains the </br> following sub-directories: code, test, personal, misc. Unless otherwise specified you are running commands from the home directory.

a.  Change directory to the test directory using absolute pathname.</br> 
    `Answer:` $ cd /home/altschool/test </br>
    ![/home/altschool/test](/Image/a..jpg)

b.  Change directory to the test directory using relative pathname. </br>
    `Answer:` $ cd test/ </br> 
    ![test/](/Image/b.jpg)

c.  Use "echo" command to create a file named fileA with text content 'Hello A' in the misc directory. </br>
    `Answer:` $ echo "Hello A" > /home/altschool/misc/fileA.txt </br>
    ![echo-"Hello-A"->-/home/altschool/misc/fileA.txt](/Image/c..jpg)

d.  Create an empty file named fileB in the misc directory. Populate the file with a dummy content </br>
    afterwards. </br>
    `Answer:`   To create an empty file: $ touch fileB.txt </br>
                To populate the file use any text editor like Vim or Nano. </br>
                $ sudo vim fileB.txt or $ sudo nano fileB.txt </br>
    ![touch-fileB.txt](/Image/d..jpg)

e.  Copy contents of fileA into fileC. </br>
    `Answer:` $ cat fileA.txt > fileC.txt </br>
    ![cat-fileA.txt->-fileC.txt](/Image/e..jpg)

f.  Move content of fileB into fileD. </br>
    `Answer:` $ sudo mv fileB.txt fileD.txt </br>
    ![sudo-mv-fileB.txt-fileD.txt](/Image/f..jpg)

g.  Create a tar acrchive called misc.tar for the contents of the misc directory. </br>
    `Answer:` $ tar -cvf misc.tar /home/altschool/misc </br>
    ![tar--cvf-misc.tar-/home/altschool/misc](/Image/g..jpg)

h.  Compress the tar archive to create a misc.tar.gz file. </br>
    `Answer:` $ tar -cvzf misc.tar.gz /home/altschool/misc </br>
    ![tar--cvzf-misc.tar.gz-/home/altschool/misc](/Image/h..jpg)

i.  Create a user and force the user to change his/her password upon login. </br>
    `Answer:` $ sudo adduser altschool2  (to create a user) </br>                                  
              And follow prompt 
    `Answer2:`To force change of password upon login do:
              $ sudo passwd -e altschool
    ![sudo-passwd--e-altschool](/Image/i..jpg)
              </div>

j.  Lock a user password. </br>
    `Answer` $ sudo passwd -l altschool2 </br>
    ![sudo-passwd--l-altschool2](/Image/j..jpg)

k.  Create a user with no login shell. </br>
    `Answer` $ sudo useradd -s /sbin/nologin altschool4 </br>
    ![sudo-useradd--s-/sbin/nologin-altschool4](/Image/k..jpg)

l.  Disable password based authentication for ssh. </br>
    `Answer` Access the ssh config directory to edit do: $ sudo vim /etc/ssh/sshd_config </br>
    ![sudo-vim-/etc/ssh/sshd_config](/Image/L(a).jpg) </br>
            change the Password Authentication or Authentication to "No" and remove comment </br>
            ![Authentication](/Image/L(b).jpg) 
            
m.  Disable root login for ssh. </br>
    `Answer:`   Access the ssh config directory to edit do:- $ sudo vim /etc/ssh/sshd_config </br>
                ![sudo-vim-/etc/ssh/sshd_config](/Image/L(a).jpg) </br>
                Locate where there is PermitRootLogin and change it to "No" and remove comment </br>
                ![PermitRootLogin](/Image/m.jpg)


