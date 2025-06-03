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

**NOTE:** To access your Foundry resource securely, please using either a VM, VPN, or ExpressRoute.