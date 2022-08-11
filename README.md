[![Deploy](https://get.pulumi.com/new/button.svg)](https://app.pulumi.com/new?template=https://github.com/pulumi/examples/blob/master/azure-py-aci/README.md)


# Pulumi

Pulumi Zero to Hero

## Create a New Project

To deploy your infrastructure, follow the below steps.

### Prerequisites

1. [Install Pulumi](https://www.pulumi.com/docs/get-started/install/)
2. [Install .NET Core 3.0+](https://dotnet.microsoft.com/download)

### Steps

1. Create a new stack:

    ```
    $ pulumi stack init dev
    ```

1. Login to Azure CLI (you will be prompted to do this during deployment if you forget this step):

    ```
    $ az login
    ```

1. Configure the location to deploy the resources to:

    ```
    $ pulumi config set azure-native:location centralus
    ```

Let’s review some of the generated project files:
.

- ```project.yaml``` is the Pulumi program that defines your stack resources.

- ```Pulumi.dev.yaml``` contains configuration values for the stack you initialized.

- ```project.yaml``` is the Pulumi program that defines your stack resources.

## Deploy the Stack

Let’s go ahead and deploy your stack:

```
pulumi up
```