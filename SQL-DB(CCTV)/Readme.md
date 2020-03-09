Step 1: Open Powershell(Run as Administrator)

Step 2: Connect-AzAccount

Step 3: Set-AzContext -SubscriptionId "3a11fa3f-8ecb-4fd6-9f79-bc8f8bc28e71"

Step 4 : New-AzResourceGroupDeployment -name "SQLServerDeployment" -ResourceGroupName CCTV-MILESTONE-RG-Test -TemplateFile "C:\Users\Saurav.srivastava\Desktop\CCTV\SQL-DB(CCTV)\template.json" -TemplateParameterFile "C:\Users\Saurav.srivastava\Desktop\CCTV\SQL-DB(CCTV)\parameters.json"
