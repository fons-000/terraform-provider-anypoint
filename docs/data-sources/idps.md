---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "anypoint_idps Data Source - terraform-provider-anypoint"
subcategory: ""
description: |-
  Reads all `identity providers` in your business group.
---

# anypoint_idps (Data Source)

Reads all `identity providers` in your business group.

## Example Usage

```terraform
data "anypoint_idps" "idp" {
  org_id = "xxxx-xxx-xxx"   # the business group id
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- **org_id** (String) The master organization id where the idps are defined.

### Optional

- **id** (String) The ID of this resource.

### Read-Only

- **idps** (List of Object) List of providers for the given org (see [below for nested schema](#nestedatt--idps))
- **total** (Number) The total number of available results

<a id="nestedatt--idps"></a>
### Nested Schema for `idps`

Read-Only:

- **name** (String)
- **org_id** (String)
- **provider_id** (String)
- **type** (Map of String)


