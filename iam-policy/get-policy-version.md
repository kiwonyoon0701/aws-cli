**Get policy as json using cli**

```
kiwony@kiwonymac.com:/Users/kiwony> aws iam get-policy-version --policy-arn arn:aws:iam::664695030410:policy/postgre-user01-policy --version-id v1|jq
{
  "PolicyVersion": {
    "Document": {
      "Version": "2012-10-17",
      "Statement": [
        {
          "Effect": "Allow",
          "Action": [
            "rds-db:connect"
          ],
          "Resource": [
            "arn:aws:rds:ap-northeast-2:664695030410:dbuser:postgre/postgre-user1"
          ]
        }
      ]
    },
    "VersionId": "v1",
    "IsDefaultVersion": true,
    "CreateDate": "2020-08-09T05:24:28+00:00"
  }
}
```

**Get policy as json and removing unnecessary rows**

```
kiwony@kiwonymac.com:/Users/kiwony> aws iam get-policy-version --policy-arn arn:aws:iam::664695030410:policy/postgre-user01-policy --version-id v1|jq |sed -e '2d;3d;16,20d'
{
      "Version": "2012-10-17",
      "Statement": [
        {
          "Effect": "Allow",
          "Action": [
            "rds-db:connect"
          ],
          "Resource": [
            "arn:aws:rds:ap-northeast-2:664695030410:dbuser:postgre/postgre-user1"
          ]
        }
      ]
}
```
