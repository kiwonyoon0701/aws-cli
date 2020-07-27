aws rds create-db-cluster --db-cluster-identifier cluster01 \
--vpc-security-group-ids sg-0f1b9ee141291034b \
--engine aurora-mysql \
--engine-version "5.7.mysql_aurora.2.08.1" \
--master-username admin \
--master-user-password <PASSWORD> \
--tags Key=Name,Value="xlarge" \
--no-storage-encrypted \
--engine-mode provisioned

aws rds create-db-instance \
--db-instance-identifier aurora01 \
--db-instance-class db.r5.2xlarge \
--engine  aurora-mysql \
--engine-version "5.7.mysql_aurora.2.08.1" \
--db-cluster-identifier cluster01 


aws rds create-db-cluster --db-cluster-identifier cluster02 \
--vpc-security-group-ids sg-0f1b9ee141291034b \
--engine aurora-mysql \
--engine-version "5.7.mysql_aurora.2.08.1" \
--master-username admin \
--master-user-password <PASSWORD> \
--tags Key=Name,Value="xlarge" \
--no-storage-encrypted \
--engine-mode provisioned

aws rds create-db-instance \
--db-instance-identifier aurora02 \
--db-instance-class db.r5.2xlarge \
--engine  aurora-mysql \
--engine-version "5.7.mysql_aurora.2.08.1" \
--db-cluster-identifier cluster02 


aws rds create-db-cluster --db-cluster-identifier cluster03 \
--vpc-security-group-ids sg-0f1b9ee141291034b \
--engine aurora-mysql \
--engine-version "5.7.mysql_aurora.2.08.1" \
--master-username admin \
--master-user-password <PASSWORD> \
--tags Key=Name,Value="4xlarge" \
--no-storage-encrypted \
--engine-mode provisioned

aws rds create-db-instance \
--db-instance-identifier aurora03 \
--db-instance-class db.r5.4xlarge \
--engine  aurora-mysql \
--engine-version "5.7.mysql_aurora.2.08.1" \
--db-cluster-identifier cluster03 



aws rds create-db-cluster --db-cluster-identifier cluster04 \
--vpc-security-group-ids sg-0f1b9ee141291034b \
--engine aurora-mysql \
--engine-version "5.7.mysql_aurora.2.08.1" \
--master-username admin \
--master-user-password <PASSWORD> \
--tags Key=Name,Value="8xlarge" \
--no-storage-encrypted \
--engine-mode provisioned

aws rds create-db-instance \
--db-instance-identifier aurora04 \
--db-instance-class db.r5.8xlarge \
--engine  aurora-mysql \
--engine-version "5.7.mysql_aurora.2.08.1" \
--db-cluster-identifier cluster04 
