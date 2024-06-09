Deployed contract using DeployWithViem.ts
command: npx ts-node --files ./scripts/DeployWithViem.ts "new prop 1" "new prop 2" "new prop 3"
TX Hash: 0x59c4b856f752d705be5339cd9f6153a17648c0c96e9f80c7c0405e6ef44a7402
Contract Address: 0x85796a059d06aafc0eb74a48a8b1a36a1e395bbe
https://sepolia.etherscan.io/address/0x85796a059d06aafc0eb74a48a8b1a36a1e395bbe

Give voting rights to second account (0x403758091A82748E6737E72F99AE36fD002B99F1)
command: npx ts-node --files ./scripts/GiveVotingRights.ts 0x85796a059d06aafc0eb74a48a8b1a36a1e395bbe 0x403758091A82748E6737E72F99AE36fD002B99F1
TX Hash: 0xa2db752c3a6dcc723726e0625811db45402877f8916ba7e34be9ccfd6b785b75
https://sepolia.etherscan.io/tx/0xa2db752c3a6dcc723726e0625811db45402877f8916ba7e34be9ccfd6b785b75

Delegate vote to chairperson
command: npx ts-node --files ./scripts/DelegateVote.ts 0x85796a059d06aafc0eb74a48a8b1a36a1e395bbe
TX Hash: 0x7392798558db503dba681b6b7635bc8b64175e81253a29900427f849d8ad4d77
https://sepolia.etherscan.io/tx/0x7392798558db503dba681b6b7635bc8b64175e81253a29900427f849d8ad4d77

Cast vote for Prop 3
command: npx ts-node --files ./scripts/CastVote.ts 0x85796a059d06aafc0eb74a48a8b1a36a1e395bbe 2
TX Hash: 0xdb8ae29cbd423bc2dee2d78daf9b995008fc5e3d598a25ed7d1a1e2c569eb4d7
https://sepolia.etherscan.io/tx/0xdb8ae29cbd423bc2dee2d78daf9b995008fc5e3d598a25ed7d1a1e2c569eb4d7

Give voting right to Andrew
command: npx ts-node --files ./scripts/GiveVotingRights.ts 0x85796a059d06aafc0eb74a48a8b1a36a1e395bbe 0x0C78fFc44616f624015366E06cbD707D4D7625a0
TX Hash: 0xfd6ae6b27c562a58a733c293659fcd67165c31e9bc5122ddc12d2844c34c57d1
https://sepolia.etherscan.io/tx/0xfd6ae6b27c562a58a733c293659fcd67165c31e9bc5122ddc12d2844c34c57d1

Andrew then delegates his vote to ChairPerson (Adrian main account)
https://sepolia.etherscan.io/tx/0xc846ef6abc80d111ff44aa91d794a928bab2acb0f87f83f502e9ec490ff05f2c
when the delegate function executes, it adds the weight of Andrew to the vote of the chairperson's proposal

Andrew then Checks the contract's propsals to see that it has 3 votes for the third propoal

```bash
➜  week2 git:(master) ✗ npx ts-node --files ./scripts/QueryResults.ts
this number should be three: 3n
```
