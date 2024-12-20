---
page_title: "FireHydrant Data Source: firehydrant_team"
subcategory: ""
---

# firehydrant_team Data Source

Use this data source to get information on a team matching the given criteria.

## Example Usage

Basic usage:

```hcl
data "firehydrant_team" "test-team" {
  id = "157a83c4-17d1-4362-a4e8-a45412d19af2"
}
```

## Argument Reference

The following arguments are supported:

* `id` - (Required) The ID of the team to retrieve.

## Attributes Reference

In addition to all arguments above, the following attributes are exported:

* `id` - The ID of the team.
* `name` - The name of the team.
* `description` - A description of the team.
* `memberships` - A set of user IDs of the members of this team
* `slug` - The slug for the team.
* `service_ids` - A set of IDs of the services associated with this team
* `owned_service_ids` - A set of IDs of the services owned by this team
