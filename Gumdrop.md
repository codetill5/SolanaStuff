# WHITELIST TOKEN CREATION
1. Minting the master edition  - number of edition 100

2. Creating a key to which we have transfer
solana keygen grind --starts-with yt:1 

solana config get / to check network

solana address -k <KEYGEN> / the key we got from the first cmd

solana airdrop <KEYGEN>

send the master edition to the <KEYGEN> via wallet

# GRUMDROP

1. ts-node packages/cli/src/gumdrop-cli.ts create 

--claim-integration edition \
--edition-mint 7Hy3FqSQYiXyg4fyobZnSJhMvAqMmraBLaTq9QSFF9ip /mint address can be get from sol expoler


# TRANSFER NFT THROUGH SPL-TOKEN CLI

spl-token transfer <SENDER_ACCOUNT_ADDRESS> <AMOUNT> <RECIPIENT_WALLET_ADDRESS> --fund-recipient

 spl-token transfer 6B199xxzw3PkAm25hGJpjj3Wj3WNYNHzDAnt1tEqg5BN 1 6VzWGL51jLebvnDifvcuEDec17sK6Wupi4gYhm5RzfkV
Transfer 1 tokens
  Sender: 6B199xxzw3PkAm25hGJpjj3Wj3WNYNHzDAnt1tEqg5BN
  Recipient: 6VzWGL51jLebvnDifvcuEDec17sK6Wupi4gYhm5RzfkV
Signature: 3R6tsog17QM8KfzbcbdP4aoMfwgo6hBggJDVy7dZPVmH2xbCWjEj31JKD53NzMrf25ChFjY7Uv2dfCDq4mGFFyAj

spl-token accounts / list all token accounts