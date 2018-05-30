# how to copy hidden files one folder up:
mv ReduxSimpleStarter/.[!.]* .

# how to delete all hidden files:
find . -name ".*" -exec rm -rf {} \;

# SSH
SSH-Copy Add public ssh key to the server:
$ssh-copy-id -i ~/.ssh/id_rsa.pub <username>@<hostname>
$ssh-copy-id -i ~/.ssh/id_rsa.pub root@director-dev

clear local history: history -c

## watch a directory:
watch "ls -l" 
for e.g.
-n 0.1 for interval 0.1 seconds
or if you want to keep the result:
while true ; do ls -l; sleep 0.1; done

## rm only subset e.g. gz and py
rm -rm *{gz,py}

# Find (and kill) process locking port 1099 on Mac
1. You can try netstat netstat -vanp tcp | grep 1099
2. For OSX El Capitan and newer (or if your netstat doesn't support -p), use lsof lsof -i tcp:1099 
