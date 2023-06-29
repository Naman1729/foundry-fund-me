# foundry-fund-me

This repository contain fund-Me in foundry framework.

## Step to flow to start foundry project for scratch

1. To get basic template of foundry framework.

```bash
  forge init
```

2. To compile the contract.

```bash
  forge compile
```

3. To deploy the contract.

- In Testnet.
  - only deploy

```bash
    forge script script/deployFundMe.s.sol --rpc-url $SEPOLIA_RPC_URL --private-key $PRIVATE_KEY --broadcast -vvvv
```

- In Testnet.
  - deploy and verify

```bash
    forge script script/deployFundMe.s.sol --rpc-url $SEPOLIA_RPC_URL --private-key $PRIVATE_KEY --broadcast --verify --etherscan-api-key $ETHERSCAN_API_KEY -vvvv
```

- In anvil.
  - To run the anvil.

```bash
  anvil
```

- In anvil.
  - deploy.

```bash
  forge script script/DeployFundMe.s.sol --rpc-url $RPC_URL --private-key $PRIVATE_KEY
```

### To test the contract.

```bash
forge test
```

### To check coverage

```bash
forge coverage
```

## For any help

- forge

```bash
  forge --help
```

and

```bash
  forge script --help
```

- cast

```bash
  cast --help
```
