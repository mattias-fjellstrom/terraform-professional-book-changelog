# Changelog for Terraform Authoring and Operations Professional Study Guide (AWS edition)

You can buy the book on [leanpub.com/terraform-professional-certification](https://leanpub.com/terraform-professional-certification).

## Changes

### 2024-11-29

* Updated all commands that export a plan file from `terraform plan -out=actions.tfplan` to `terraform plan -out="actions.tfplan"` due to the command not working on Powershell without the quotation marks. Updated the corresponding `terraform apply` commands as well.
* Added a default value of `eu-west-1` for the variable block in Figure 3.35.
* Extended the list of names in Acknowledgments

### 2024-10-23

* Extended the example and discussion around `locals` in chapter 4.
* Added an additional deciding factor between `for_each` and `count` in the discussion around these meta-arguments in chapter 4.
* Clarified the description around nullable variables in chapter 4.
* Removed the `key` attribute for the `backend` block in Figure 5.27.
* Updated the text following Figure 6.17 to refer to the correct module path.
* Clarified the example around `terraform_remote_state` to clearly talk about a producer configuration and a consumer configuration.

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