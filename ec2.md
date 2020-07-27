aws ec2 run-instances \
--image-id ami-023a41b4b0c4c25db \
--instance-type c4.4xlarge \
--key-name id_rsa_main \
--monitoring Enabled=true \
--security-group-ids sg-05ea43a464458a4f0 \
--iam-instance-profile Name=MySSMRole \
--tag-specifications 'ResourceType=instance,Tags=[{Key=Name,Value=Oracle01}]'
