aws dms create-replication-task \
--replication-task-identifier mig01 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:YARIYJU3BMOUG576NEFJPPICMMS22F2WWCOOUFQ \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:EVUY4OXIPEMSH6FVQ6GP6Z5RDXRBX3NSWDM7ITQ \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:6PYMAMWLUC2DYG7TJOP7TKFOEPHMBY2HB5JLR7I \
--migration-type full-load \
--replication-task-settings file://replication-task.json \
--table-mappings file://table01.json

### Oracle2

aws dms create-replication-task \
--replication-task-identifier mig02-1 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:B3YRHUJBIIMCZJ673Y4ELMW67TSS6Q75SSHSZ4Q \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:JKPTXMC5K4XXXCDTWZIF2JXWYKGRELGXCDUHSRA \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:U55RTYTBDZDQFSQYOY7ZJQBLW6K5IPMDEPHRGRI \
--migration-type full-load \
--replication-task-settings file://replication-task.json \
--table-mappings file://table02-01.json

aws dms create-replication-task \
--replication-task-identifier mig02-2 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:B3YRHUJBIIMCZJ673Y4ELMW67TSS6Q75SSHSZ4Q \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:JKPTXMC5K4XXXCDTWZIF2JXWYKGRELGXCDUHSRA \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:U55RTYTBDZDQFSQYOY7ZJQBLW6K5IPMDEPHRGRI \
--migration-type full-load \
--replication-task-settings file://replication-task.json \
--table-mappings file://table02-02.json

### oracle03

aws dms create-replication-task \
--replication-task-identifier mig03-1 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:C4XS65LYLBXDAHAHWSOT3ZHU74X6TF5LY5VCI5Q \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:4JK27H2WPHNLVLRTYFR4CUY5S3QGTHH7MMIPSGQ \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:LJBODY7FU7YV4VTTTZ44PAL5YACQZPQKKQ3MFIQ \
--migration-type full-load \
--replication-task-settings file://replication-task49.json \
--table-mappings file://table03-01.json

aws dms create-replication-task \
--replication-task-identifier mig03-2 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:C4XS65LYLBXDAHAHWSOT3ZHU74X6TF5LY5VCI5Q \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:4JK27H2WPHNLVLRTYFR4CUY5S3QGTHH7MMIPSGQ \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:LJBODY7FU7YV4VTTTZ44PAL5YACQZPQKKQ3MFIQ \
--migration-type full-load \
--replication-task-settings file://replication-task49.json \
--table-mappings file://table03-02.json

### oracle04

aws dms create-replication-task \
--replication-task-identifier mig04-1 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:KGHTHBR4WCLXMCTSUIV2Z3CIM7OGLJ72PX3NO5Y \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:CWDGWI6CBN3VOLUSGMLPJMTSI5KWEJN6CIAD2BI \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:I5UH53B44KHLKJ7SELAFOP6JY43L4L3HV2QRE3I \
--migration-type full-load \
--replication-task-settings file://replication-task49.json \
--table-mappings file://table04-01.json

aws dms create-replication-task \
--replication-task-identifier mig04-2 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:KGHTHBR4WCLXMCTSUIV2Z3CIM7OGLJ72PX3NO5Y \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:CWDGWI6CBN3VOLUSGMLPJMTSI5KWEJN6CIAD2BI \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:I5UH53B44KHLKJ7SELAFOP6JY43L4L3HV2QRE3I \
--migration-type full-load \
--replication-task-settings file://replication-task49.json \
--table-mappings file://table04-02.json

aws dms create-replication-task \
--replication-task-identifier mig04-3 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:KGHTHBR4WCLXMCTSUIV2Z3CIM7OGLJ72PX3NO5Y \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:CWDGWI6CBN3VOLUSGMLPJMTSI5KWEJN6CIAD2BI \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:I5UH53B44KHLKJ7SELAFOP6JY43L4L3HV2QRE3I \
--migration-type full-load \
--replication-task-settings file://replication-task49.json \
--table-mappings file://table04-03.json

aws dms create-replication-task \
--replication-task-identifier mig04-4 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:KGHTHBR4WCLXMCTSUIV2Z3CIM7OGLJ72PX3NO5Y \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:CWDGWI6CBN3VOLUSGMLPJMTSI5KWEJN6CIAD2BI \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:I5UH53B44KHLKJ7SELAFOP6JY43L4L3HV2QRE3I \
--migration-type full-load \
--replication-task-settings file://replication-task49.json \
--table-mappings file://table04-04.json

aws dms create-replication-task \
--replication-task-identifier mig01 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:YARIYJU3BMOUG576NEFJPPICMMS22F2WWCOOUFQ \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:EVUY4OXIPEMSH6FVQ6GP6Z5RDXRBX3NSWDM7ITQ \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:6PYMAMWLUC2DYG7TJOP7TKFOEPHMBY2HB5JLR7I \
--migration-type full-load \
--replication-task-settings file://replication-task.json \
--table-mappings file://table01.json

### Oracle2

aws dms create-replication-task \
--replication-task-identifier mig02-1 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:B3YRHUJBIIMCZJ673Y4ELMW67TSS6Q75SSHSZ4Q \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:JKPTXMC5K4XXXCDTWZIF2JXWYKGRELGXCDUHSRA \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:U55RTYTBDZDQFSQYOY7ZJQBLW6K5IPMDEPHRGRI \
--migration-type full-load \
--replication-task-settings file://replication-task.json \
--table-mappings file://table02-01.json

aws dms create-replication-task \
--replication-task-identifier mig02-2 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:B3YRHUJBIIMCZJ673Y4ELMW67TSS6Q75SSHSZ4Q \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:JKPTXMC5K4XXXCDTWZIF2JXWYKGRELGXCDUHSRA \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:U55RTYTBDZDQFSQYOY7ZJQBLW6K5IPMDEPHRGRI \
--migration-type full-load \
--replication-task-settings file://replication-task.json \
--table-mappings file://table02-02.json

### oracle03

aws dms create-replication-task \
--replication-task-identifier mig03-1 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:C4XS65LYLBXDAHAHWSOT3ZHU74X6TF5LY5VCI5Q \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:4JK27H2WPHNLVLRTYFR4CUY5S3QGTHH7MMIPSGQ \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:LJBODY7FU7YV4VTTTZ44PAL5YACQZPQKKQ3MFIQ \
--migration-type full-load \
--replication-task-settings file://replication-task49.json \
--table-mappings file://table03-01.json

aws dms create-replication-task \
--replication-task-identifier mig03-2 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:C4XS65LYLBXDAHAHWSOT3ZHU74X6TF5LY5VCI5Q \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:4JK27H2WPHNLVLRTYFR4CUY5S3QGTHH7MMIPSGQ \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:LJBODY7FU7YV4VTTTZ44PAL5YACQZPQKKQ3MFIQ \
--migration-type full-load \
--replication-task-settings file://replication-task49.json \
--table-mappings file://table03-02.json

### oracle04

aws dms create-replication-task \
--replication-task-identifier mig04-1 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:KGHTHBR4WCLXMCTSUIV2Z3CIM7OGLJ72PX3NO5Y \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:CWDGWI6CBN3VOLUSGMLPJMTSI5KWEJN6CIAD2BI \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:I5UH53B44KHLKJ7SELAFOP6JY43L4L3HV2QRE3I \
--migration-type full-load \
--replication-task-settings file://replication-task49.json \
--table-mappings file://table04-01.json

aws dms create-replication-task \
--replication-task-identifier mig04-2 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:KGHTHBR4WCLXMCTSUIV2Z3CIM7OGLJ72PX3NO5Y \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:CWDGWI6CBN3VOLUSGMLPJMTSI5KWEJN6CIAD2BI \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:I5UH53B44KHLKJ7SELAFOP6JY43L4L3HV2QRE3I \
--migration-type full-load \
--replication-task-settings file://replication-task49.json \
--table-mappings file://table04-02.json

aws dms create-replication-task \
--replication-task-identifier mig04-3 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:KGHTHBR4WCLXMCTSUIV2Z3CIM7OGLJ72PX3NO5Y \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:CWDGWI6CBN3VOLUSGMLPJMTSI5KWEJN6CIAD2BI \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:I5UH53B44KHLKJ7SELAFOP6JY43L4L3HV2QRE3I \
--migration-type full-load \
--replication-task-settings file://replication-task49.json \
--table-mappings file://table04-03.json

aws dms create-replication-task \
--replication-task-identifier mig04-4 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:KGHTHBR4WCLXMCTSUIV2Z3CIM7OGLJ72PX3NO5Y \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:CWDGWI6CBN3VOLUSGMLPJMTSI5KWEJN6CIAD2BI \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:I5UH53B44KHLKJ7SELAFOP6JY43L4L3HV2QRE3I \
--migration-type full-load \
--replication-task-settings file://replication-task49.json \
--table-mappings file://table04-04.json

aws dms create-replication-task \
--replication-task-identifier mig01 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:YARIYJU3BMOUG576NEFJPPICMMS22F2WWCOOUFQ \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:EVUY4OXIPEMSH6FVQ6GP6Z5RDXRBX3NSWDM7ITQ \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:6PYMAMWLUC2DYG7TJOP7TKFOEPHMBY2HB5JLR7I \
--migration-type full-load \
--replication-task-settings file://task10.json \
--table-mappings file://table-mapping.json

aws dms create-replication-task \
--replication-task-identifier mig02 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:B3YRHUJBIIMCZJ673Y4ELMW67TSS6Q75SSHSZ4Q \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:JKPTXMC5K4XXXCDTWZIF2JXWYKGRELGXCDUHSRA \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:U55RTYTBDZDQFSQYOY7ZJQBLW6K5IPMDEPHRGRI \
--migration-type full-load \
--replication-task-settings file://task20.json \
--table-mappings file://table-mapping.json

aws dms create-replication-task \
--replication-task-identifier mig03 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:C4XS65LYLBXDAHAHWSOT3ZHU74X6TF5LY5VCI5Q \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:4JK27H2WPHNLVLRTYFR4CUY5S3QGTHH7MMIPSGQ \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:LJBODY7FU7YV4VTTTZ44PAL5YACQZPQKKQ3MFIQ \
--migration-type full-load \
--replication-task-settings file://task30.json \
--table-mappings file://table-mapping.json

aws dms create-replication-task \
--replication-task-identifier mig04 \
--source-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:KGHTHBR4WCLXMCTSUIV2Z3CIM7OGLJ72PX3NO5Y \
--target-endpoint-arn arn:aws:dms:ap-northeast-2:664695030410:endpoint:CWDGWI6CBN3VOLUSGMLPJMTSI5KWEJN6CIAD2BI \
--replication-instance-arn arn:aws:dms:ap-northeast-2:664695030410:rep:I5UH53B44KHLKJ7SELAFOP6JY43L4L3HV2QRE3I \
--migration-type full-load \
--replication-task-settings file://task40.json \
--table-mappings file://table-mapping.json
