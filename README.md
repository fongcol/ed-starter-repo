**Description**

  - This sample elasticdev file performs CI with docker exclusively on AWS/Ec2.  It will automatically create the ecr_repo for your docker images. If the ecr_repo exists, you can remove that section in the yml.  However, you can leave it and it will not do anything if the repo already exists.

  - Please be sure to provide for the location of the "Dockerfile" and "Dockerfile_test" relative to the code repository.  If Dockerfile_test is not provided, it will skip any elementary testing.  

  - Please note, this is for basic CI.  For more complex CIs, feel free to use the BuildKite CI stack that will be coming out soon.  

**files**

```
elasticdev_temple.yml - copy the file and filled the fields in "<>". 
```

```
elasticdev_example.yml - a example that is works
```
