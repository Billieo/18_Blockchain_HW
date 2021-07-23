# 18_Blockchain_HW
The following tools and software are  needed for the POA algorithm.

Go Ethereum [Go Ethereum's Website](https://geth.ethereum.org/downloads/)

MyCrypto [Crypto's Website](https://download.mycrypto.com/)


To start your block on a POA algorithm, you need to create two account that will be seal and prefunded during the puppeth configuration. To create this two account or node you will use the following command. 

### code for creating new account 
* ./geth --datadir node1 account new
* ./geth --datadir node2 account new

you will need to save your Public address of the key for both node1 and node2.


## Puppeth configuration
For this section we will be using puppeth which comes with the blockchain download.

### code for executing puppeth
* ./puppeth

The following prompt will come up
- Specify your network name.
- Select 2 to configure genesis block.
- Select 1 to create new genesis from scratch.
- Select 2 for Clique - proof-of-authority.
- Click enter to select the default time which is 15mins.
- Paste in node 1 and 2 address for account allowed to be sealed.
- Paste in node 1 and 2 address for account to be pre-funded.
- Select 2, manager existing genesis.
- Export genesis configuration.


![alttext](image/Puppet_configuration_1.png)
![alttext](image/Puppet_configuration_2.png)


init node
![alttext](image/Initnode.png)

## Connecting to the network
- While you node are running open Crypto account.
- Scroll to the button of the page and click change network and then select add custon node.

### Setting up custom node
 - Node name: is the name of the network you selected during puppet configuration.
 - Network name: is the name of the network.
 - Network: scroll down in the drop box and select custom.
 - Port: we are going to use http://127.0.0.1:8545
 - The click save and use custom node.

  ![alttext](image/custom_node.png)

 - Click change network again to change to the new network you just created.

 ![alttext](image/changing_network.png)
 - Click the keystore 
 - Select node 1
 - Copy and paste node 2 address in the sent to address. 
 - Use the slider to select the transaction fee for your transaction.
 - Submit the transaction.

### Check Transaction status.
- After submitting a transacting go back in the terminal and you should see a submitted transaction. 
- Once you see the submitted transaction, click on TX Status or you can click on check status or the green bar at the bottom of the check transaction status window.

  ![alttext](image/check_transaction_status.png)

Transaction sucessfully sent confirmation
  ![alttext](image/transaction_confirmation.png)