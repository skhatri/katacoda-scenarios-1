Use the clouddrive command
In Cloud Shell, you can run a command called clouddrive, which enables you to manually update the file share that is mounted to Cloud Shell. Running the "clouddrive" command

List clouddrive
To discover which file share is mounted as clouddrive, run the df command.

The file path to clouddrive shows your storage account name and file share in the URL. For example, //storageaccountname.file.core.windows.net/filesharename


```
justin@Azure:~$ df
Filesystem                                          1K-blocks   Used  Available Use% Mounted on
overlay                                             29711408 5577940   24117084  19% /
tmpfs                                                 986716       0     986716   0% /dev
tmpfs                                                 986716       0     986716   0% /sys/fs/cgroup
/dev/sda1                                           29711408 5577940   24117084  19% /etc/hosts
shm                                                    65536       0      65536   0% /dev/shm
//mystoragename.file.core.windows.net/fileshareName 5368709120    64 5368709056   1% /home/justin/clouddrive
justin@Azure:~$
```