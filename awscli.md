# Awscli
install awscli below:
```
# yum install awscli -y
```
And connect to iam user aws:
```
# aws configure
AWS Access Key ID [None]: AKIA3IOSICEKNRQXPZGE
AWS Secret Access Key [None]: Q8sivf5lwpi7x79A16Tz2E9G+FTN6j4H4d5HGUMg
Default region name [None]: eu-central-1
Default output format [None]: json
```
Command examples:
```
# aws s3 ls
2022-06-23 13:26:25 muradsamadov-bucket
2022-06-23 13:20:42 muradsamadov-bucket-it-logs
```
Above list available s3 buckets. If you dont know command use 'help' command as below:
```
# aws help
# aws s3 ls help
```
Below commmand list all files at  'muradsamadov-bucket' bucket
```
# aws s3 ls s3://muradsamadov-bucket
2022-06-22 16:14:25      93987 163-1632819_png-extension-download-iconos-con-extension-ico-transparent.png
2022-06-22 15:49:43     174377 antalya.jpg
2022-06-22 15:07:04          8 awsfile
2022-06-23 08:48:47      35944 clouds.jpg
2022-06-23 08:48:46        255 error.html
2022-06-23 08:48:45        526 index.html
2022-06-22 16:30:52         14 testfile.txt
```
