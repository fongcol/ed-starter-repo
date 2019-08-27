**Description**

  - This sample elasticdev file creates a VPC with essentially 2 security groups - database and web/api - as opposed to 3 tier Web Application.  Though it is meant to be used for development, it can also be used for production.

**Notable**
  -  Ports open to public include: 

```
  http: 8090-9010 
  ssh: 22000-22500
```

**Required**

| argument      | description                            | var type | default      |
| ------------- | -------------------------------------- | -------- | ------------ |
| vpc_name   | name of the vpc                 | string   | None         |

**Optional**

| argument      | description                            | var type | default      |
| ------------- | -------------------------------------- | -------- | ------------ |
| region   | AWS region to create the vpc                 | string   | us-east-1         |
