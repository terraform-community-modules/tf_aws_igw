Internet Gateway Terraform module
=================================

A Terraform module to provide an Internet Gateway in AWS.


Module Input Variables
----------------------

- `vpc_id` - vpc id
- `name` - name (optional)
- `tags` - dictionary of tags that will be added to resources created by the module

Usage
-----

```js
module "igw" {
  source = "github.com/terraform-community-modules/tf_aws_igw"

  name   = "default"
  vpc_id = "vpc-12345678"

  tags {
    "Terraform" = "true"
    "Environment" = "${var.environment}"
  }
}
```

Outputs
=======

 - `igw_id` - igw id

Authors
=======

Originally created and maintained by [Anton Babenko](https://github.com/antonbabenko)

License
=======

Apache 2 Licensed. See LICENSE for full details.
