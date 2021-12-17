## Projects
## **TODO** Project 0
together: what resources/configs do we need if we create a online magazine?
    1. server
    2. hard drive
    3. storage for images
    4. cdn/caching
    5. database
    6. security (e.g. vpn, private subnets, firewalls) (pbb, we want to separte admin/public areas)
    7. dns, ssl
    8. deployments methods
    9. ANALYTICS AND ALERTING TOOLS
    10. snapshots/backups
    11. data analysis
## **TODO** Project 1/2
- `aws iam create-group --group-name content-managers-2`
- `aws iam attach-group-policy --policy-arn arn:aws:iam::aws:policy/AmazonS3FullAccess --group-name content-managers-2`
- `aws iam create-user --user-name content-manager-2`
- `aws iam create-login-profile --user-name content-manager-2 --password My!User1Login8P@ssword --password-reset-required`
- `aws iam add-user-to-group --user-name content-manager-2 --group-name content-manager-2`

## **TODO** Project 3
- Launch instance `aws ec2 run-instances --image-id ami-0d527b8c289b4af7f  --instance-type t2.micro --security-group-ids [xxx] --subnet-id [xxx]--key-name aws-devops-project --user-data file://install-apache2.txt`
- Terminate instance `aws ec2 terminate-instances --instance-ids [xxx]`
- Launch DB isntance `aws rds create-db-instance --db-instance-identifier test-mysql-instance --db-instance-class db.t2.micro     --engine mysql --master-username admin --master-user-password secret99 --allocated-storage 20`
- Connect to DB from server `mysql -h database-1.czxmicpeeunr.eu-central-1.rds.amazonaws.com -u admin -p`
- List databases `show databases`;

## **TODO** Project 4


## **TODO** Project 5