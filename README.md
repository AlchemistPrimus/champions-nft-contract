# Champions NFT  
Minting an NFT using Anchor and Metaplex on solana blockchain network.  

## Testing the project on the devnet  
#### Prerequisites  
Ensure you have enough SOL balance in your wallet for this deployment. If not, 
on the devnet run `solana airdrop 2` to get some.  

Configuring the validator.  
`$ solana config set --url localhost`  

### Building, deploying and testing the program  
```
    $ anchor build  
    $ anchor keys list // Returns key that we replace in the declare_id!() macro and Anchor.toml config.  
    $ anchor build // Run anchor build again now that we have the right keys.  
    $ anchor deploy  // Deploying the project on the blockchain.  
    $ anchor test --skip-build --skip-deploy // --skip-build and --skip-deploy optional flags are added since we had already done the actions.
```

The NFT has now been minted on the blockchain.
