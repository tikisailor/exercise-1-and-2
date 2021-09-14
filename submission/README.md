# Substrate Runtime Developer Academy

## Exercise One

1. Setup development environment
2. Fork & clone this project
3. Update author in Cargo.toml file
4. Run a single node testnet and send a transaction

### Testnet

![Testnet image](testnet.png?raw=true "Running testnet")

### Transaction

![Transaction image](transaction.png?raw=true "Transaction")


---

## Exercise Two

1. Design kitties pallet
2. Requirements:
    - Kitty must have a 128 bit DNA, which is randomly generated
    - Kitty must have one owner
    - A user can have zero or more kitties
    - Users can create kitties

### Design

Storages
    - Kitties_record: map AccountId => Vec<Kitty:u128>

Calls
    - fn create_kitty(AccountId)
        - kitty = OffchainWorker random u128
        - fn assign_owner(AccountId, kitty)


---
