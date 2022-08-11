# Pulumi

Pulumi Zero to Hero

# Create a New Project

```
mkdir quickstart && cd quickstart
pulumi new azure-yaml
```

To list all available locations, use the az account list-locations command.

```
az account list-locations --output table
```

You can then change the region for your stack by using the pulumi config set command as shown below:

```
pulumi config set azure-native:location eastus
```

Let’s review some of the generated project files:

Pulumi.yaml defines both the project and the program that manages your stack resources.
Pulumi.dev.yaml contains configuration values for the stack you initialized.

# Deploy the Stack

Let’s go ahead and deploy your stack:

```
pulumi up
```