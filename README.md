**Description**

  - This sample elasticdev file creates a VPC with essentially 2 security groups - database and web/api - as opposed to 3 tier Web Application.  Though it is meant to be used for development, it can also be used for production.  The stack contained in the sample configuration will also handle the creationo of the high available subnets, route tables, and internet gateways.

**Notable**
  -  Ports open to public include: 

```
  http: 8090-9010 
  ssh: 22000-22500
  vpc_name: <project_name>-vpc
```

**Optional**

| argument      | description                            | var type | default      |
| ------------- | -------------------------------------- | -------- | ------------ |
| region   | AWS region to create the vpc                 | string   | us-east-1         |
