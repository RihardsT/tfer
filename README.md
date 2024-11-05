### About
Simple Terraform wrapper script to achieve "*include*".  
This should allow to organize Terraform code without using modules.

Only example for now: https://github.com/RihardsT/cloud_project_terraform_oracle

### Install
Either copy or link the script from the repo
```
sudo ln -s ${PWD}/tfer /usr/bin/tfer
```

### To do:
- [x] Flag to only create links
- [x] Flag to change Terraform dir
- [x] Refactor - check file diff and add/remove links as needed
- [x] If the same filename is in multiple folders, link with `_` -> folder_file
      Or maybe just link all files like that: folder_file,
      even within multiple folders
- [ ] As `terraform.tfvars` is the default vars for Terraform,
      it doesn't work with the `_` naming (folder_file).
      The script should not look for `*.tfvars`,
      just link the default `terraform.tfvars`.
      Other `tfvars` should be taken from `-var-file=../FILE` anyway
- [ ] Check for duplicate links
- [ ] This needs tests in general and regression tests too
- [ ] TODO
- [ ] TODO
