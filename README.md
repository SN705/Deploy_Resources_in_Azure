Fictional Dental Clinic - Repository for CICD Deployment of Azure Resources

This repository contains a masterworkflow.yaml file that is triggered by changes in all branches including itself. The workflow deploys resources to a fictional Dental Clinic Azure tenant named Dino Smiles by authenticating via repository secrets. Each branch in the repository represents the creation of a separate service. Any changes made to the branch script or parameter files will automatically be pushed to Azure. The Create_Resource_Group branch specifically contains variables that can be modified in the parameters.json file. Once the changes are committed, a new resource group will be created automatically in Azure.

Workflow Details

masterworkflow.yml: The workflow file that is triggered by changes in all branches, including changes in its own file.
Create_Resource_Group: The branch that contains the parameters.json file where variables can be modified for the creation of a new resource group in Azure.
secrets.: References to the repository secrets used for authentication to the Azure tenant.
env.: The environment variables used in the workflow file to pass parameters to the Azure CLI commands.
az cli: The Azure CLI command-line interface used to deploy resources to the Dino Smiles Azure tenant.
