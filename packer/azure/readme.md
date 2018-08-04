

# 

chefdk-2.5.3-1.dmg
gem install kitchen-azurerm


```
0  (master *) $ kitchen test
-----> Starting Kitchen (v1.20.0)
-----> Cleaning up any prior instances of <default-azure-xenial64>
-----> Destroying <default-azure-xenial64>...
       Finished destroying <default-azure-xenial64> (0m0.00s).
-----> Testing <default-azure-xenial64>
-----> Creating <default-azure-xenial64>...
/Users/alvaro/.azure/credentials was not found or not accessible.
       Creating Resource Group: kitchen-default-azure-xenial64-20180804T220500
       Creating deployment: deploy-5a50e3e714009dcc
       Adding public key from /Users/alvaro/.ssh/id_rsa.pub to the deployment.
       Resource Microsoft.Network/virtualNetworks 'vnet' provisioning status is Running
       Resource Microsoft.Resources/deployments 'pid-18d63047-6cdf-4f34-beed-62f01fc73fc2' provisioning status is Running
       Resource Microsoft.Compute/virtualMachines 'myvm' provisioning status is Running
       Resource Microsoft.Compute/virtualMachines 'myvm' provisioning status is Running
       Resource Microsoft.Compute/virtualMachines 'myvm' provisioning status is Running
       Resource Microsoft.Compute/virtualMachines 'myvm' provisioning status is Running
       Resource Microsoft.Compute/virtualMachines 'myvm' provisioning status is Running
       Resource Template deployment reached end state of 'Succeeded'.
       IP Address is: 137.116.118.220 [kitchen-5a50e3e714009dcc.eastus.cloudapp.azure.com]
       Finished creating <default-azure-xenial64> (2m38.28s).
-----> Converging <default-azure-xenial64>...
       Preparing files for transfer
       Preparing script
       No provisioner script file specified, skipping
       Transferring files to <default-azure-xenial64>
       Downloading files from <default-azure-xenial64>
       Finished converging <default-azure-xenial64> (0m7.54s).
-----> Setting up <default-azure-xenial64>...
       Finished setting up <default-azure-xenial64> (0m0.00s).
-----> Verifying <default-azure-xenial64>...
       Loaded tests from {:path=>".Users.alvaro.Downloads.packer_xenial64.azure.test.integration.default"} 

Profile: tests from {:path=>"/Users/alvaro/Downloads/packer_xenial64/azure/test/integration/default"} (tests from {:path=>".Users.alvaro.Downloads.packer_xenial64.azure.test.integration.default"})
Version: (not specified)
Target:  ssh://azure@137.116.118.220:22

  System Package wget
     ✔  should be installed

Test Summary: 1 successful, 0 failures, 0 skipped
       Finished verifying <default-azure-xenial64> (0m3.19s).
-----> Destroying <default-azure-xenial64>...
/Users/alvaro/.azure/credentials was not found or not accessible.
       Azure environment: Azure
       Destroying Resource Group: kitchen-default-azure-xenial64-20180804T220500
       Destroy operation accepted and will continue in the background.
       Finished destroying <default-azure-xenial64> (0m37.62s).
       Finished testing <default-azure-xenial64> (3m26.66s).
-----> Kitchen is finished. (3m30.53s)
0  (master *) $
```