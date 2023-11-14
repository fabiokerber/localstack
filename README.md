## Links
https://docs.localstack.cloud/user-guide/integrations/kubernetes/
https://docs.localstack.cloud/getting-started/installation/#helm
https://docs.localstack.cloud/tutorials/
https://docs.localstack.cloud/tutorials/s3-static-website-terraform
https://artifacthub.io/packages/helm/localstack/localstack
https://github.com/localstack/awscli-local

## Helm Values
```
https://github.com/localstack/helm-charts/blob/main/charts/localstack/values.yaml
```

## ssh ubuntu_kind
```
k get pods -o wide
k get nodes -o wide
export AWS_ENDPOINT_URL=http://172.18.0.4:31566
awslocal s3api create-bucket --bucket testwebsite
awslocal s3api list-buckets
```

## /etc/hosts
```
cat << EOF >> /etc/hosts
192.168.56.180 localstack.fks.lab
EOF
```

## Navegador > http://localstack.fks.lab
