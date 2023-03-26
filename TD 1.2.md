# Exercice 1
1. sudo apt update
2. uname -r
3. top
4. ps
5. nproc
6. lscpu
7. df
8. mount
9. lsblk
10. hostname

# Exercice 2
1. x="piri pimpin"
2. echo $x
3. x+=" piri pimpon"
4. mkdir my_programs
5. cd my_programs
6. vim pilou
7. source pilou
8. chmod u+x pilou
9. ./pilou
10. echo $PATH
11. PATH=$PATH:$(pwd)
12. export PATH
13. cd ~
14. pilou
15. PATH="$PATH:$HOME/my_programs"
16. source .profile
17. pilou

# Exercice 3
1. vim say_hello.sh
2. chmod +x say_hello.sh
3. crontab -e

# Exercice 4
1. mkdir hash_checksum
2. cd hash_checksum/
3. touch .sensible_addresses 
4. touch .sensible_passwords
5. ls -a
6. nano gentle_script.sh
7. source gentle_script.sh
8. sha256sum gentle_script.sh > log_sha
9. echo "rm -rf .sensible*" >> gentle_script.sh
10. sha256sum gentle_script.sh >> log_sha
11. source gentle_script
12. ls -a
13. cat log_sha
