## Terraform Recommendations

A quick note. [Terraform recommends](https://www.terraform.io/docs/cloud/guides/recommended-practices/part1.html) managing infrastructure in smaller Terraform configurations.

> You shouldn't use a single Terraform workspace to manage everything that makes up your production or staging environment. Instead, make smaller workspaces that are easy to delegate. One Workspace Per Environment Per Terraform Configuration.

A workspace provides a "namespace" for all the resources contained in an environment and configuration. Essentially, you create separate workspaces with separate statefiles.
