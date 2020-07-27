## Create recpliation instance
aws dms create-replication-instance \
--replication-instance-identifier ri-c4xlarge \
--replication-instance-class dms.c4.xlarge \
--no-multi-az \
--engine-version "3.4.0" \
--no-publicly-accessible 

## Create Endpoint
### Target Endpoint
aws dms   create-endpoint \
--endpoint-identifier target-aurora01 \
--endpoint-type target \
--engine-name aurora \
--username admin \
--password <PASSWORD> \
--server-name cluster01.cluster-cf89zyffo8dr.ap-northeast-2.rds.amazonaws.com \
--port 3306 


--password abcc
