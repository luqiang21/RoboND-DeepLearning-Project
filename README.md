command to upload files to the AWS instance
scp -i "robond.pem" your_file ubuntu@ec2-54-212-223-139.us-west-2.compute.amazonaws.com:~/.

unzip files to a specific folders
unzip file.zip -d your_target_folder
