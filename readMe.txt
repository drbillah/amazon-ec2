Check CUDA version
$ nvcc --version
$ ls -alh /usr/local/cuda

login to the server:
ssh -i "***.pem" user@ip

Copy file local computer to ec2:
scp -i "***.pem" ubuntu@ec2-ip:path /path/file/test.txt

scp -i "masum.pem" /home/drbillah/master/lab/data/concat/images.zip ubuntu@ec2-ip:~/payload/tools/darknet/goat/




To copy from EC2 to S3 use the below code in the Command line of EC2.

First, you have to give "IAM Role with full s3 Access" to your EC2 instance.

aws s3 cp Your_Ec2_Folder s3://Your_S3_bucket/Your_folder --recursive

aws s3 cp filelocation/filename s3://bucketname
