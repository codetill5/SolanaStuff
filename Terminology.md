### SPL: Solana Program Language

Spl token can be seen as the token standard for the solana blockchain. Spl tokens are to solana what ERC-20, ERC-721 and ERC-1155 tokens are to the Ethereum network.

ERC-20  standard regulates fungible tokens
ERC-721 NFTs
ERC-1155 semi fungible tokens.

spl-token create-token

spl-token supply <token-identifier>

The initial supply should be zero as we haven’t added anything to the token. But, worry not, we’ll show you how to add a supply of your desired amount. However, before actually minting the supply, we do need to create an account for the program. The reason for manually adding this is that programs on the Solana blockchain don’t generally have any storage by default. As such, we need to add the account ourselves






--------------------------------------------------------------------------------

In Solana there is simply one program defining the common implementation of both fungible tokens and NFTs.

lamports: tiny fractions of a SOL token
PDA: Program Derived Account Address
RPC: Remote Procedure Call:  form of an API which allows developers to communicate to a server in order to remotely execute code