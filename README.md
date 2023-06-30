# SNS-service-using-cli

1. Configure aws
   
 aws configure

2. Create an SNS Topic

aws sns create-topic --name YourTopicName

3. Set topic display name

aws sns set-topic-attributes --topic-arn YourTopicARN --attribute-name DisplayName --attribute-value YourDisplayName

4. Add subscription to the topic

aws sns subscribe --topic-arn YourTopicARN --protocol email --notification-endpoint YourEmailAddress

5. Publish a message to the topic

aws sns publish --topic-arn YourTopicARN --message "Hello, SNS!"
