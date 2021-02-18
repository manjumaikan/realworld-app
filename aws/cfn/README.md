To-do tasks

copy elastic.repo,GPG_KEY-elasticsearch and filebeat.yaml to an S3 bucket and make the changes to cfn templates

realworld-api.yaml and realworld-web.yaml
    aws s3 cp s3://<<bucket-name>>/GPG-KEY-elasticsearch  /etc/elastic/
    aws s3 cp s3://<<bucket-name>>/elastic.repo /etc/yum.repos.d/
    aws s3 cp s3://<<bucket-name>>/filebeat.yaml /etc/filebeat/filebeat.yml
