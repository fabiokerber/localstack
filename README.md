## Links
https://docs.localstack.cloud/user-guide/integrations/kubernetes/<br>
https://docs.localstack.cloud/getting-started/installation/#helm<br>
https://docs.localstack.cloud/tutorials/<br>
https://docs.localstack.cloud/tutorials/s3-static-website-terraform<br>
https://artifacthub.io/packages/helm/localstack/localstack<br>
https://github.com/localstack/awscli-local<br>
https://docs.localstack.cloud/user-guide/aws/elastic-compute-cloud/<br>

## Helm Values
```
https://github.com/localstack/helm-charts/blob/main/charts/localstack/values.yaml
```

## ssh ubuntu_kind
```
kubens awslocal
k get pods -o wide
k get nodes -o wide
export AWS_ENDPOINT_URL=http://172.18.0.4:31566
awslocal s3api create-bucket --bucket testwebsite
awslocal s3api list-buckets
awslocal s3 ls
```

## /etc/hosts
```
cat << EOF >> /etc/hosts
192.168.56.180 localstack.fks.lab
EOF
```

## Navegador > http://localstack.fks.lab
