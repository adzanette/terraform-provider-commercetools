---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "commercetools_shipping_zone Resource - terraform-provider-commercetools"
subcategory: ""
description: |-
  
---

# commercetools_shipping_zone (Resource)



## Example Usage

```terraform
resource "commercetools_shipping_zone" "de-us" {
  name = "DE and US"
  description = "Germany and US"
  location {
      country = "DE"
  }
  location {
      country = "US"
      state = "Nevada"
  }
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- **description** (String)
- **id** (String) The ID of this resource.
- **key** (String)
- **location** (Block List) (see [below for nested schema](#nestedblock--location))
- **name** (String)

### Read-Only

- **version** (Number)

<a id="nestedblock--location"></a>
### Nested Schema for `location`

Required:

- **country** (String)

Optional:

- **state** (String)

