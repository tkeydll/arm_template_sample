# Azure Resource Manager Sample

## Minimum Template

### Storage Account

```json
        {
            "type": "Microsoft.Storage/storageAccounts",
            "sku": {
                "name": "Standard_LRS",
                "tier": "Standard"
            },
            "name": "[parameters('storageAccountName')]",
            "apiVersion": "2018-07-01",
            "location": "[resourceGroup().location]"
        }
```

