Here are some of the main Terraform commands you'll commonly use in your infrastructure deployment workflow:

1. **`terraform init`**: Initializes a new or existing Terraform configuration. This command downloads the necessary providers and sets up the working directory.
    
    `terraform init`
    
2. **`terraform plan`**: Generates an execution plan describing what Terraform will do to reach the desired state specified in your configuration files. It's a good practice to run this before applying changes to understand the impact.
3. 
    `terraform plan`
    
3. **`terraform apply`**: Applies the changes described in a Terraform execution plan. This command is used to create or modify resources according to the Terraform configuration.

    `terraform apply`
    
    If you want to auto-approve changes without being prompted, you can use:
    
    `terraform apply -auto-approve`
    
4. **`terraform destroy`**: Destroys the infrastructure defined by the Terraform configuration. It's important to use this command with caution, as it will delete resources.
    
    `terraform destroy`
    
    Similar to `apply`, you can auto-approve destruction:
    
    `terraform destroy -auto-approve`
    
5. **`terraform validate`**: Validates the syntax and format of the Terraform files in the current directory.
    
    `terraform validate`
    
6. **`terraform fmt`**: Rewrites Terraform configuration files to a canonical format. This helps maintain consistent code style.
    
    `terraform fmt`
    
7. **`terraform state`**: Manages the Terraform state. This includes various subcommands like `terraform state list`, `terraform state show`, and `terraform state pull`. It allows you to inspect and manage the state of your infrastructure. For more information check [[Terraform state]].
    
    `terraform state list`
    
8. **`terraform refresh`**: Updates the state file to match the real-world resources.
    
    `terraform refresh`
    
9. **`terraform output`**: Displays output values defined in your Terraform configuration.
    
    `terraform output`

These are some of the fundamental Terraform commands. Depending on your use case and the complexity of your infrastructure, you may use additional commands and features such as modules, variables, and remote backends. Always refer to the [official Terraform documentation](https://www.terraform.io/docs/cli/commands/index.html) for detailed information and examples.