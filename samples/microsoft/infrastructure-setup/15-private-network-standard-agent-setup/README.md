# Azure AI Agent Service: Standard Agent Setup with Private E2E Networking

> **NOTE:** This template is to set-up a network secured Standard Agent in AI Foundry. Includes:
* PNA disabled resources
* PE's to all resources
* Network injection enabled for Agents

## Steps

1. Create new (or use existing) resource group:

```bash
    az group create --name <new-rg-name> --location <your-rg-region>
```

2. Deploy the main.bicep

```bash
    az deployment group create --resource-group <new-rg-name> --template-file main.bicep
```

[![Deploy To Azure](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmeerakurup%2Ffoundry-samples%2Fb25bdfd5c308f1ae8bc4f41759e73bb229292529%2Fsamples%2Fmicrosoft%2Finfrastructure-setup%2F15-private-network-standard-agent-setup%2Fmain.json)

**NOTE:** To access your Foundry resource securely, please using either a VM, VPN, or ExpressRoute.