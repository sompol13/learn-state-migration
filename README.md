## Migrate State to Terraform Cloud
As a current user of the Terraform CLI, you are responsible for maintaining a state file as a source of truth for your cloud infrastructure. *You can keep your state file secure and share it with collaborators, by migrating it to Terraform Cloud without interrupting or recreating your existing infrastructure.*

### Create state (Local)
- `terraform init`
- `terraform apply`
- Terraform will output a three word randomly generated pet name.

### Reference
https://learn.hashicorp.com/tutorials/terraform/cloud-migrate#set-up-the-remote-backend
