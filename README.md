# ApiGW-UsagePlan-with-ApiKey
```
API-GW rate limit for Usage Plans with API Key usage
```

# Creating Components
```
aws cloudformation create-stack --template-body file://./rate-limit.yml --cli-input-yaml file://./initial-parameter.yml
```

# Updating Components
```
aws cloudformation update-stack --template-body file://./rate-limit.yml --cli-input-yaml file://./initial-parameter.yml
```

# Destrying Components
```
aws cloudformation delete-stack --stack-name  rate-limit-poc
```
