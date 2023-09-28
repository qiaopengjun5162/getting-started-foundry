## Foundry

**Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.**

Foundry consists of:

- **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
- **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
- **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
- **Chisel**: Fast, utilitarian, and verbose solidity REPL.

## Documentation

<https://book.getfoundry.sh/>

## Usage

### Build

```shell
forge build
```

### Test

```shell
forge test
```

### Format

```shell
forge fmt
```

### Gas Snapshots

```shell
forge snapshot
```

### Anvil

```shell
anvil
```

### Deploy

```shell
forge script script/Counter.s.sol:CounterScript --rpc-url <your_rpc_url> --private-key <your_private_key>
```

### Cast

```shell
cast <subcommand>
```

### Help

```shell
forge --help
anvil --help
cast --help
```

## getting-started-foundry

```shell
3704* mcd foundry-projects
3705* forge init getting-started-foundry
3706* ls
3707* cd getting-started-foundry/
3708* code .

3750* forge build
3751* touch remappings.txt
3752* forge remappings
3753* forge build
3754* forge remappings
3755* forge test
3756* forge build
3757* anvil
3758* export PRIVATE_KEY=0xac0974bec39a17e36ba4a6b4d238ff944bacb478cbed5efcae784d7bf4f2ff80

3760* forge create src/Counter.sol:Counter --private-key=$PRIVATE_KEY
3761* cast --help
3762* cast balance 0x5fbdb2315678afecb367f032d93f642f64180aa3
3763* cast call 0x5fbdb2315678afecb367f032d93f642f64180aa3 "getNumber()(uint256)"

3765* cast send 0x5fbdb2315678afecb367f032d93f642f64180aa3 "setNumber(uint256)" 4 --private-key=$PRIVATE_KEY
3766* cast call 0x5fbdb2315678afecb367f032d93f642f64180aa3 "getNumber()(uint256)"
3767* echo "# getting-started-foundry" >> README.md
```
