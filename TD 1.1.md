# TD1: Use basic Linux commands

# Exericice 1
cd /
ls -a
pwd

#1
mkdir test
cd /home
cd 
cd ~
cd ..
cd ..
cd

#2
mkdir test
cd test
pwd

# Exercise 2: Create, Rename, copy, delete
cd
pwd

#3
mkdir linux_ex_1
cd linux_ex_1

#4
vim Franck.txt

#5
mkdir notes
mv Franck.txt notes/

#6
mv Franck.txt Franck_2023.txt

#7
cp -r notes notes_2022

#8
rm -rv notes

# Exercise 3: Create and run a script
vim script_1.sh
#!/bin/bash
echo "Script running please wait ..."
echo "Done."

#9
cat script_1.sh

#10
source script_1.sh

#11
bash script_1.sh

# Exercise 4: Accessing or modifying a file : permissions and root privilege

# Exercise 4.1
vim credentials
cat credentials
ls -l credentials

#12
chmod a-w credentials
ls -l credentials

#13
vim credentials
cat credentials

#14
chmod a+rw credentials
ls -l credentials

#15
vim credentials
cat credentials

#16
chmod u+x credentials
ls -l credentials

#17
chmod o-r credentials
ls -l credentials

#18
chmod a=rwx credentials
ls -l credentials

# Exercise 4.2
sudo su -
touch .private_file
sudo vim .private_file
sudo cat .private_file
vim .private_file
cat .private_file

#19
sudo vim .private_file
sudo cat .private_file

#20
sudo chmod 777 .private_file
vim .private_file
cat .private_file

# Exercise 4.3
chmod a+rw .private_file

#21
sudo chown $USER .private_file
chmod a+rw .private_file

# Exercise 4.4
sudo apt update
sudo apt upgrade
sudo apt install cmatrix
cmatrix
Ctrl + C
sudo apt install tmux
tmux

#22
echo "Hello session 0"
cmatrix
Ctrl + B
puis d

#23
tmux new -s mysession
echo "Hello session 1"
Ctrl + B
puis d

#24
tmux ls
tmux attach-session -t 0
