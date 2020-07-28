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

### Source Endpoint
aws dms   create-endpoint \
--endpoint-identifier OnPREM-Oracle001 \
--endpoint-type source \
--engine-name oracle \
--username dms_user \
--password <PASSWORD> \
--database-name salesdb \
--port 1521 \
--server-name 172.31.20.159

aws dms test-connection \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:6PYMAMWLUC2DYG7TJOP7TKFOEPHMBY2HB5JLR7I \
--endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:YARIYJU3BMOUG576NEFJPPICMMS22F2WWCOOUFQ

aws dms test-connection \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:U55RTYTBDZDQFSQYOY7ZJQBLW6K5IPMDEPHRGRI \
--endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:B3YRHUJBIIMCZJ673Y4ELMW67TSS6Q75SSHSZ4Q

aws dms test-connection \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:B4UQ7GQ2P7TV2LPDLEVMVLATFFNHJL5SJYPIO7I \
--endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:C4XS65LYLBXDAHAHWSOT3ZHU74X6TF5LY5VCI5Q

aws dms test-connection \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:FVLND6TMKMMEBRZJJAT52YXXBZD3FUAHYYKQOAY \
--endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:KGHTHBR4WCLXMCTSUIV2Z3CIM7OGLJ72PX3NO5Y


aws dms create-replication-task \
--replication-task-identifier mig01 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:YARIYJU3BMOUG576NEFJPPICMMS22F2WWCOOUFQ \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:EVUY4OXIPEMSH6FVQ6GP6Z5RDXRBX3NSWDM7ITQ \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:6PYMAMWLUC2DYG7TJOP7TKFOEPHMBY2HB5JLR7I \
--migration-type  full-load \
--replication-task-settings file://replication-task.json \
--table-mappings file://table-mapping.json

aws dms create-replication-task \
--replication-task-identifier mig02 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:B3YRHUJBIIMCZJ673Y4ELMW67TSS6Q75SSHSZ4Q \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:JKPTXMC5K4XXXCDTWZIF2JXWYKGRELGXCDUHSRA \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:U55RTYTBDZDQFSQYOY7ZJQBLW6K5IPMDEPHRGRI \
--migration-type  full-load \
--replication-task-settings file://replication-task.json \
--table-mappings file://table-mapping.json

aws dms create-replication-task \
--replication-task-identifier mig03 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:C4XS65LYLBXDAHAHWSOT3ZHU74X6TF5LY5VCI5Q \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:4JK27H2WPHNLVLRTYFR4CUY5S3QGTHH7MMIPSGQ \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:LJBODY7FU7YV4VTTTZ44PAL5YACQZPQKKQ3MFIQ \
--migration-type  full-load \
--replication-task-settings file://replication-task.json \
--table-mappings file://table-mapping.json

aws dms create-replication-task \
--replication-task-identifier mig04 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:KGHTHBR4WCLXMCTSUIV2Z3CIM7OGLJ72PX3NO5Y \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:CWDGWI6CBN3VOLUSGMLPJMTSI5KWEJN6CIAD2BI \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:I5UH53B44KHLKJ7SELAFOP6JY43L4L3HV2QRE3I \
--migration-type  full-load \
--replication-task-settings file://replication-task.json \
--table-mappings file://table-mapping.json


aws dms modify-replication-instance \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:6PYMAMWLUC2DYG7TJOP7TKFOEPHMBY2HB5JLR7I \
--apply-immediately \
--replication-instance-class dms.c4.2xlarge \
--no-multi-az \
--replication-instance-identifier ri-c4xlarge01	

aws dms modify-replication-instance \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:U55RTYTBDZDQFSQYOY7ZJQBLW6K5IPMDEPHRGRI \
--apply-immediately \
--replication-instance-class dms.c4.2xlarge \
--no-multi-az \
--replication-instance-identifier ri-c4xlarge02	

aws dms modify-replication-instance \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:B4UQ7GQ2P7TV2LPDLEVMVLATFFNHJL5SJYPIO7I \
--apply-immediately \
--replication-instance-class dms.c4.2xlarge \
--no-multi-az \
--replication-instance-identifier ri-c4xlarge03	

aws dms modify-replication-instance \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:FVLND6TMKMMEBRZJJAT52YXXBZD3FUAHYYKQOAY \
--apply-immediately \
--replication-instance-class dms.c4.2xlarge \
--no-multi-az \
--replication-instance-identifier ri-c4xlarge04	

arn:aws:dms:ap-northeast-2:664695030410:rep:6PYMAMWLUC2DYG7TJOP7TKFOEPHMBY2HB5JLR7I
arn:aws:dms:ap-northeast-2:664695030410:rep:U55RTYTBDZDQFSQYOY7ZJQBLW6K5IPMDEPHRGRI
arn:aws:dms:ap-northeast-2:664695030410:rep:LJBODY7FU7YV4VTTTZ44PAL5YACQZPQKKQ3MFIQ
arn:aws:dms:ap-northeast-2:664695030410:rep:I5UH53B44KHLKJ7SELAFOP6JY43L4L3HV2QRE3I


aws dms create-replication-instance \
--replication-instance-identifier ri-c4xlarge004 \
--replication-instance-class dms.c4.2xlarge \
--no-multi-az \
--engine-version "3.4.0" \
--no-publicly-accessible
