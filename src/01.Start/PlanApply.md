# Terraform Plan and Apply

terraform plan

Expected output:

```
Terraform used the selected providers to generate the following execution plan. Resource actions are indicated with the following symbols:       
  + create

Terraform will perform the following actions:

  # azurerm_resource_group.first_tf will be created
  + resource "azurerm_resource_group" "first_tf" {
      + id       = (known after apply)
      + location = "uksouth"
      + name     = "first_tf_rgp"
    }

Plan: 1 to add, 0 to change, 0 to destroy.
```

terraform apply

Expected output:

```
azurerm_resource_group.first_tf: Creating...
azurerm_resource_group.first_tf: Creation complete after 0s [id=/subscriptions/******/resourceGroups/first_tf_rgp]

Apply complete! Resources: 1 added, 0 changed, 0 destroyed.
```
