vesting.token
-----------

This eosio contract allows users to create, issue, and manage tokens on
eosio based blockchains.

Vesting token contract extends the basic eosio.token with an option to vest tokens for some amount of time (from 1 second to aprox 10 years). For now `vest` action is allowed only to the contract owner itself (_self auth is requered to vest).

When the vesting period ends the reciepent can `claimvest` to get his tokens. The `from` param should be the same as the `to` param in `vest` action.