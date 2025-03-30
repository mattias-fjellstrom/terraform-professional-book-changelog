# Changelog for Terraform Authoring and Operations Professional Study Guide

You can buy the digital edition of the book on Leanpub (delivered as both PDF and ePUB):

* [AWS edition](https://leanpub.com/terraform-professional-certification).

## Changes

### AWS edition

#### 2025-03-30

* Fix formatting issues discovered in printed version of the book.
* Updated wording in a few sentences throughout the book.
* Added a footnote concerning updates to AWS S3 backend.
* Replaced footnote link with a QR code for LinkedIn.
* Changed text color for output boxes in Terraform diagrams from white to black for better contrast.
* Updated colors on the cover to include AWS orange (`#FF9900`)
* Fixed minor typos.

#### 2025-01-21

* Fix minor typos in a CLI command based on feedback
* Resized a few images to fit the page better

#### 2025-01-04

This update is focused on the look-and-feel of the book, not on the technical content. This is in preparation for a printed edition of this book.

* Updated the book format from A4 (210x297 mm) to technical trade (178x254 mm).
* Changed from gray-scale to color for all code snippets.
* Added a _Preface_ chapter in Part 1 of the book, thus renumbering the following chapters.
* Moved the final words to its own final chapter.
* Updated the accompanying sample repo to reflect the new chapter numbers and updated all the links in the book.
* Updated screenshots in Chapter 3 (previously Chapter 2) due to updates to the look-and-feel of the AWS console.
* Changed from using variables sets in HCP Terraform to using workspace variables in the example in Chapter 3. Removed a number of screenshots and some explanations due to this change.
* Split the **JSON, YAML, CSV** aside into three separate asides because Leanpub could not generate one long aside without splitting it in weird ways across three pages.
* Split the **Locals** aside into two separate asides (same reason as above).
* Updated the GitHub repository references to be in the text instead of as footnotes. This is because in the print-ready PDF markdown links to websites are generated as footnotes.
* Deleted a few superfluous footnotes that did not add any value.
* General formatting of the book to look nice, this includes adding page-breaks, truncating output, resizing images, etc.
* Moved _Target audience_ and _Visual elements of this book_ to the Introduction chapter.

#### 2024-12-11

* Added a sample code repository at [github.com/mattias-fjellstrom/terraform-professional-book-sample-code](https://github.com/mattias-fjellstrom/terraform-professional-book-sample-code).
* Included references to the GitHub repository from the corresponding code samples in the book.
* Added a subsection mentioning the GitHub repository in Chapter 1.
* Replaced the _Terraform provider ecosystem_ image in Chapter 7.

#### 2024-11-29

* Updated all commands that export a plan file from `terraform plan -out=actions.tfplan` to `terraform plan -out="actions.tfplan"` due to the command not working on Powershell without the quotation marks. Updated the corresponding `terraform apply` commands as well.
* Added a default value of `eu-west-1` for the variable block in Figure 3.35.
* Extended the list of names in Acknowledgments

#### 2024-10-23

* Extended the example and discussion around `locals` in chapter 4.
* Added an additional deciding factor between `for_each` and `count` in the discussion around these meta-arguments in chapter 4.
* Clarified the description around nullable variables in chapter 4.
* Removed the `key` attribute for the `backend` block in Figure 5.27.
* Updated the text following Figure 6.17 to refer to the correct module path.
* Clarified the example around `terraform_remote_state` to clearly talk about a producer configuration and a consumer configuration.

#### 2024-10-08

* Fixed the `dynamic` block example in Figure 4.47. The `local.ports` value was used as a list of objects in the `dynamic` block, even though it was a list of numbers.
* Added an explicit `aws_vpc` resource to the example in Figure 4.47.
* Added a new example in Figure 4.48 for a `dynamic` block using a map.
* Updated the `terraform show` command in Figure 3.8 to pipe the output from `terraform show` to `jq` for better formatting.
* Added a default value for the `aws_region` variable in Figure 3.15.
* Added a default value for the `aws_region` variable in Figure 3.24.
* Updated the description around the example in Figure 3.24 to tell the reader to recreate the infrastructure that was previously destroyed.
* Extended the example around Figure 3.32, 3.33, and 3.34 with clarifications for how to import a resource into your state and have Terraform generate the configuration for you.
* Extended the list of names in Acknowledgments

#### 2024-10-02

* Initial book release