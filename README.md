**Description**

  - This sample elasticdev file creates an AMI when provided instance_id and copy it to regions if specified.
  - A label is required by the platform to version an application.  For example, a label could be "bob_store_front" to reference the contents of the AMI image.  The first creation of the AMI image is 1.  The second time you create an image with the same label, its version will be 2, 3, etc. This is useful when you want to control you deploys, saying for example we are on version 5 of bob_store_front, but need to rollback to contents in version 4.  In the ED stack, you can specify version 4, and it will automatically grab the name of the ami image accordingly.


**Optional**

| argument      | description                            | var type | default      |
| ------------- | -------------------------------------- | -------- | ------------ |
| instance_id   | instance_id to create AMI with                 | string   | None         |
| aws_default_region   | AWS region                  | string   | us-east-1         |
| label   | a label is needed to automatically version ami images.  | string   | us-east-1         |

**Optional**

| argument      | description                            | var type | default      |
| ------------- | -------------------------------------- | -------- | ------------ |
| copy_regions   | regions to copy the image                 | string   | None         |
| encrypted   | Set True if you want the AMI image encrypted       | boolean   | None       |

**files**

```
elasticdev_temple.yml - copy the file and filled the fields in "<>". 
```

```
elasticdev_example.yml - a example that is works
```
