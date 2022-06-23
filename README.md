# ApiGW-UsagePlan-with-ApiKey without Log & Monitoring
```
# API-GW rate limit for Usage Plans with API Key usage
```
without Log & Monitoring with Log & Monitoring


# Creating Components without Log & Monitoring
```
aws cloudformation create-stack --template-body file://./rate-limit.yml --cli-input-yaml file://./initial-parameter.yml
```

# Creating Components with Log & Monitoring
```
aws cloudformation create-stack --template-body file://./rate-limitcw.yml --cli-input-yaml file://./initial-paramete-cw.yml
```

# Updating Components without Log & Monitoring
```
aws cloudformation update-stack --template-body file://./rate-limit.yml --cli-input-yaml file://./initial-parameter.yml
```
# Updating Components with Log & Monitoring
```
aws cloudformation update-stack --template-body file://./rate-limit-cw.yml --cli-input-yaml file://./initial-parameter-cw.yml
```

# Destrying Components for the stack that has no Log & Monitoring
```
aws cloudformation delete-stack --stack-name  rate-limit-poc
```

# Destrying Components for the stack that has Log & Monitoring
```
aws cloudformation delete-stack --stack-name  rate-limit-poc-cw
```
