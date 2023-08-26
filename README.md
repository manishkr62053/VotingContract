# VotingContract Smart Contract

This is a simple Solidity smart contract that simulates a basic voting system. The contract allows users to vote for candidates and provides functionality to check vote counts and close the voting process.

## Contract Overview

The VotingContract smart contract has the following features:

- Each voter can vote for a candidate only once.
- The contract keeps track of the vote count for each candidate.
- The owner of the contract can close the voting process, preventing further modifications.
- The contract rejects incoming Ether transactions.

## Usage

1. **Deploy the Contract:** Deploy the `VotingContract` smart contract on an Ethereum-compatible blockchain network (such as Ganache for local testing or a testnet/mainnet for production).

2. **Interact with the Contract:** Use the contract functions to interact with it:

   - `vote(string memory candidate)`: Allows a user to cast their vote for a candidate. Users can vote only once.
   - `getVoteCount(string memory candidate)`: Retrieves the current vote count for a specific candidate.
   - `closeVoting()`: Closes the voting process. Only the contract owner can call this function after ensuring there is at least one candidate.

3. **Total Candidates:** The function `getTotalCandidates()` returns the total number of candidates. In this example, it's hardcoded to 1, but in a real scenario, you would dynamically determine the total number of candidates.

4. **Ether Transactions:** The contract rejects incoming Ether transactions to ensure that it doesn't accept any Ether.

## Ownership and Security

The contract uses the `onlyOwner` modifier to ensure that certain functions can only be called by the owner of the contract. This helps prevent unauthorized modifications.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Note

This smart contract is intended for educational purposes and is not audited for production use. Always ensure proper testing and security measures before deploying to a live network.
