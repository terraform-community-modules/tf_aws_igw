IGW Terraform module
====================

A Terraform module to provide an Internet Gateway in AWS.


Module Input Variables
----------------------

- `vpc_id` - VPC id
- `name` - Name (optional)

Usage
-----

```js
module "igw" {
  source = "github.com/terraform-community-modules/tf_aws_igw"

  name   = "default"
  vpc_id = "vpc-12345678"
}
```

Outputs
=======

 - `igw_id` - IGW id

Authors
=======

Originally created and maintained in [hashicorp/atlas-examples](https://github.com/hashicorp/atlas-examples/tree/master/infrastructures/terraform/aws/network/igw).
Hijacked by [Anton Babenko](https://github.com/antonbabenko)

License
=======

Apache 2 Licensed. See LICENSE for full details.