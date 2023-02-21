Write a smart contract that allows users to deposit 2 tokens in a 1:1 ratio, and deposits those tokens into two separate strategy contracts, one per deposit denom. This contract should  support Bonding, StartUnbonding and Unbonding, on Unbond the funds should be returned to the user.

To test your contract’s interactions with the other contract, write an appropriate test where you mock the strategy contract. You can copy the above code snippets and import them in your contract. You may always assume happy flow in the Strategy contract when the local denom is correct and the time between StartUnbondResponse and Unbond is correct.

-------------------------------------------------------------------------
cargo build --target wasm32-unknown-unknown --lib

cargo wasm  

cargo test

cargo run schema