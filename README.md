## Migrate State to Terraform Cloud
As a current user of the Terraform CLI, you are responsible for maintaining a state file as a source of truth for your cloud infrastructure. *You can keep your state file secure and share it with collaborators, by migrating it to Terraform Cloud without interrupting or recreating your existing infrastructure.*

### Create state (Local)
- `terraform init`
- `terraform apply`
- Terraform will output a three word randomly generated pet name.

### Set up Terraform Cloud
Now that you have a local state file, you need to create a `cloud` code block in your configuration.

### Migrate the state file
- `terraform init`
- Configure the Terraform Cloud workspace.
- Add variable `name_length` to the workspace

### Initiate a run in the new workspace
- After verifying that the state was migrated to the Terraform Cloud workspace, remove the local state file.
- `rm terraform.tfstate`
- `terraform apply`
- 

<img width="1384" alt="Screen Shot 2565-01-29 at 13 52 42" src="https://user-images.githubusercontent.com/33342822/151651217-9ca4b9fe-8771-4fb5-a8ec-76ff7f27a254.png">

### Reference
https://learn.hashicorp.com/tutorials/terraform/cloud-migrate#set-up-the-remote-backend
