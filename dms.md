## Create recpliation instance
aws dms create-replication-instance \
--replication-instance-identifier ri-c4xlarge \
--replication-instance-class dms.c4.xlarge \
--no-multi-az \
--engine-version "3.4.0" \
--no-publicly-accessible 

