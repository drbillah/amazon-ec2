Check CUDA version
$ nvcc --version
$ ls -alh /usr/local/cuda

Crate partitation:
$ sudo fdisk /dev/xvdb
 Then press: p (partitation)
Output -> Disk /dev/xvdb
Then press : n (new)
Output: partition type..
Then press: p
Then press: enter
Then press: enter
Then press: enter
Output: Create a new partition 1
Then press: w

$ sudo mkfs.ext4 /dev/xvdb1
$ cd 
$ mkdir payload
$ sudo mount /dev/xvdb1 payload
$ df -h
$ sudo chmod a+rwx payload
$ cd payload/
$ touch foo
$ ls -alh
