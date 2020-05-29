---
title: Tfvars
---

config/terraform.tfvars

```terraform
account_name = "my account"
region = "us-west-2"
```

## Materialization

When you run `terraspace` commands, it will use the files in the config folder and materialized withdeployed module.  For example, let's say you have an `app/modules/instance` module:

    .
    │── app
    │   └── modules
    │       └── instance
    └── config
        └── terraform.tfvars

Running:

    terraspace build instance

Builds a `.terrspace-cache/dev/modules/instance/terraform.tfvars` using the `config/terraform.tfvars`. This is useful if you want to have to set the same tfvars in all your modules.