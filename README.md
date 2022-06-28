# git commands

## clone -> clone repos from online to local machine
## add -> allow git to take note of your recent changes
## commit -> save your files in giy
## push -> upload your git commits to a remote repo
## pull -> download changes form a remote repo to a local machine

# How to check for git and git versions
## git --version
 ---> git version 2.37.0.windows.1

# how to pull a repo to an offline machine
1st. with VScode goto view>terminal or open cmd from root folder dir
 
# Check if SSH exists
## ls -al ~/.ssh
    total 9
    drwxr-xr-x 1 DELL 197121  0 Jun 27 17:51 ./
    drwxr-xr-x 1 DELL 197121  0 Jun 27 17:58 ../
    -rw-r--r-- 1 DELL 197121 92 Jun 27 17:51 known_hosts
# to change dir to the ssh directory
 ##    cd ~/.ssh
---> DELL@DESKTOP-Q2PCHUC MINGW64 ~/.ssh
# CHECK IF AN OLD ONE EXISTS
## $ cat id_rsa.pub
---> cat: id_rsa.pub: No such file or directory

--root-> DELL@DESKTOP-Q2PCHUC MINGW64 ~/.ssh,
# create new private/public ssh
## $ ssh-keygen -t ed25519 -C "yakubmuhammed51@gmail.com"

Generating public/private ed25519 key pair.
Enter file in which to save the key (/c/Users/DELL/.ssh/id_ed25519):
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Passphrases do not match.  Try again.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/DELL/.ssh/id_ed25519
Your public key has been saved in /c/Users/DELL/.ssh/id_ed25519.pub
The key fingerprint is:
SHA256:MnnQgjZs6E8/+6ss0XsMPnMJCEaeTNxUJhirof6B0cg yakubmuhammed51@gmail.com
The key's randomart image is:
+--[ED25519 256]--+
| ..=o.o          |
|  =+.+ .         |
|.=o.* o .        |
|o+Oo . +         |
|oE.o.o+ S        |
|. ooo.++         |
| o ..oo= .       |
|  . o.=o=        |
|   . .+Bo.       |
+----[SHA256]-----+

DELL@DESKTOP-Q2PCHUC MINGW64 ~/.ssh
# start the ssh-agent in the background
## $ eval "$(ssh-agent -s)"
---> Agent pid 1147
# Add pid agent id
## $ ssh-add ~/.ssh/id_ed25519
Enter passphrase for /c/Users/DELL/.ssh/id_ed25519:
Identity added: /c/Users/DELL/.ssh/id_ed25519 (yakubmuhammed51@gmail.com)
DELL@DESKTOP-Q2PCHUC MINGW64 ~/.ssh

# Generate and copy the agent ssh to your clipboard
## $ clip < ~/.ssh/id_ed25519.pub
# Now go to github and paste the id


# HOW TO CHECK STATUS OF OUR REPOS
## git status

# HOW TO ADD CHANGES MADE TO GIT [. MEANS EVERYTHING EVERY CHANGES, INDEX.HTML MEANS ONLY IT]
## git add .

# how to commit Changes to be committed: 