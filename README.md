# ubuntu-server-trash-installation

 system update & trash-cli package 
```bash

sudo apt-get update

sudo apt-get install trash-cli
```
 Edit .bashrc File:
 ```bash
nano ~/.bashrc
```
 Add the Following Code at the End of the File:
 ```
alias rm='trash'
```
Apply Changes to .bashrc File:
```
source ~/.bashrc
```
Test the Trash System
```
touch testfile.txt
```
Delete the File Using rm:
```
rm testfile.txt
```
. Check the Trash Folder:
```
trash-list
```
```bash
cd ~/.local/share/Trash/files/
ls
```
Example output:
testfile.txt

