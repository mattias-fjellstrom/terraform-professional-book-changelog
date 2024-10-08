# Changelog for Terraform Authoring and Operations Professional Study Guide (AWS edition)

You can buy the book on [leanpub.com/terraform-professional-certification](https://leanpub.com/terraform-professional-certification).

## Changes

### 2024-10-08

* Fixed the `dynamic` block example in Figure 4.47. The `local.ports` value was used as a list of objects in the `dynamic` block, even though it was a list of numbers.
* Added an explicit `aws_vpc` resource to the example in Figure 4.47.
* Added a new example in Figure 4.48 for a `dynamic` block using a map.
* Updated the `terraform show` command in Figure 3.8 to pipe the output from `terraform show` to `jq` for better formatting.
* Added a default value for the `aws_region` variable in Figure 3.15.
* Added a default value for the `aws_region` variable in Figure 3.24.
* Updated the description around the example in Figure 3.24 to tell the reader to recreate the infrastructure that was previously destroyed.
* Extended the example around Figure 3.32, 3.33, and 3.34 with clarifications for how to import a resource into your state and have Terraform generate the configuration for you.
* Extended the list of names in Acknowledgments

### 2024-10-02

* Initial book release