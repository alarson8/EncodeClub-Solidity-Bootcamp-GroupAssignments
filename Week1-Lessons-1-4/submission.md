[Week 1 Assignment](https://github.com/alarson8/EncodeClub-Solidity-Bootcamp-GroupAssignments.git)

```    
This is a group activity for at least 3 students:

Interact with “HelloWorld.sol” within your group to change message strings and change owners

Write a report with each function execution and the transaction hash, if successful, or the revert reason, if failed
    
Submit your weekend project by filling the form provided in Discord
```

---------------
Current Contributors:   
```
LmdPqy - zig (Andrew)
kdM4Jd - Adrian_Caso
93vCgT - Canaima
```
---------------
Current Submission:
1.	Andrew Deployed the contract, started at .25sEth

https://sepolia.etherscan.io/tx/0x2e9da65b58b339ec7df2f9a16ed985d0afd15559253546969c4c42599a243aff


2.	Andrew Clicked HelloWorld, had 0.2491sEth from deploy and was at no cost to click HelloWorld

3.	Andrew Clicked SetText, with "this is my text that is going to go over the limit for array elements to show" some had .2491 Seth, now have .2490

https://sepolia.etherscan.io/tx/0xe0b242cbfb238eed6fd3e127a0afcc50ccd2490290d095ba8b4254f918671211

4.	Adrian used the “Connect Wallet” from the environment tab dropdown, then added the contract address to the "At Address" button within the Deploy and Transact. Adrian then clicked the HelloWorld button and saw Andrew's previously set, “Set Text” of “…this is my text”.

5.	Adrian starts at .9093 sEth, and clicked SetText. Adrian received a Gas Estimation failed error highlighting Adrian was not currently the owner. Adrian Clicked to send the transaction and again, MetaMask warned that the transaction was likely to fail; which it did. 

https://sepolia.etherscan.io/tx/0x46d72383b58214ac3a652bb35e48e54b0f004e9d18bf53c318e64da7ece0b3bd

6.	Andrew changes ownership using the failed from address within the previous transaction to set Adrian as the owner

https://sepolia.etherscan.io/tx/0x453022ede314b2fdfee0b3706b93128c7b1ff3fe6f1c50a6c2a66914ce38d30c

7.	 With Adrian as the owner, when Adrian clicked SetText he was able to change the text to “Adrian is the the owner”

https://sepolia.etherscan.io/tx/0xed6ac3fb91a0d4aa0a34b0663c6ac1c57414e2e36d8fffef9ba430420b67de35


8.	When clicking “HelloWolrd” Adrian and Andrew both see the changed text of “Adrian is the owner”

9.	With Adrian as the owner, Andrew now tried to set text to “Andrew is now the owner”, received exact same messaging from both Remix and MetaMask that the transaction was likely to fail; which it subsequently did.

https://sepolia.etherscan.io/tx/0xf3d76146dc4af83bfaada4666de29cf193dceea4d51d0a442b05bd008f140e43


10. Shijin accessed contract at 0x089d2927a6ae42fc657cdfd9fc681e9c31d55d42 and saw the message set by Adrian ("Adrian is the owner of this contract")

11. Shijin called the setText field and received an error (only owner) 

https://sepolia.etherscan.io/tx/0x2038400f08fe62e50e7272675d44dc69aca24afa4ff8c0062c98f8a6a8fd0b25

12. Adrian transferred ownership to Shijin. 

https://sepolia.etherscan.io/tx/0x5b786cd2a4d03cf7289c680bed491bcfbf25bd1416a143102aca92de290660c4

13. Shijin setText to "Shijin is the owner". 

https://sepolia.etherscan.io/tx/0xe2ce3df3787f294af84558446e86dc6effa661054473a5985abc55ed57229869
  