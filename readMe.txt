Check CUDA version
$ nvcc --version
$ ls -alh /usr/local/cuda

login to the server:
ssh -i "***.pem" user@ip

Copy file local computer to ec2:
scp -i "***.pem" ubuntu@ec2-ip:path /path/file/test.txt

scp -i "masum.pem" /home/drbillah/master/lab/data/concat/images.zip ubuntu@ec2-ip:~/payload/tools/darknet/goat/
