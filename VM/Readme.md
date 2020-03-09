Step 1: Open Powershell(Run as Administrator)

Step 2: Connect-AzAccount

Step 3: Set-AzContext -SubscriptionId "3a11fa3f-8ecb-4fd6-9f79-bc8f8bc28e71"

Step 4 : New-AzResourceGroupDeployment -name "VMDeployment" -ResourceGroupName CCTV-MILESTONE-RG-Test -TemplateFile "C:\Users\Saurav.srivastava\Desktop\CCTV\VM\template.json" -TemplateParameterFile "C:\Users\Saurav.srivastava\Desktop\CCTV\VM\parameters.json"

Note: If you want to use this file again for deployment please change the value of Subnet and Vnet in the parameters.json file


        "subnetName": {
            "value": "S061-NOE-subnet"
        },
        "virtualNetworkId": {
            "value": "/subscriptions/3a11fa3f-8ecb-4fd6-9f79-bc8f8bc28e71/resourceGroups/S061-NOE-network/providers/Microsoft.Network/virtualNetworks/S061-NOE-vnet"
        }

                                        TO.....

        "subnetName": {
            "value": "S017-NOE-subnet"
        },
        "virtualNetworkId": {
            "value": "/subscriptions/0216b091-a611-45eb-ba48-1854302c9509/resourceGroups/S017-NOE-network/providers/Microsoft.Network/virtualNetworks/S017-NOE-vnet"
        }