Step 1: Open Powershell(Run as Administrator)

Step 2: Connect-AzAccount

Step 3: Set-AzContext -SubscriptionId "0216b091-a611-45eb-ba48-1854302c9509"

Step 4 : New-AzResourceGroupDeployment -name "SQLServerDeployment" -ResourceGroupName SCRUBBER-RG-Prod -TemplateFile "C:\Users\Saurav.srivastava\Desktop\Workshop\Scrubber\SQL-DB\template.json" -TemplateParameterFile "C:\Users\Saurav.srivastava\Desktop\Workshop\Scrubber\SQL-DB\parameters.json"
