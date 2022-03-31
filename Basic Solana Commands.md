### Check Current Network
solana config get

### change network
solana config set --url https://api.devnet.solana.com

### creating new wallet
solana-keygen new

Note: The above command will first ask for a passphrase, it will just be for a security purpose, if we do not want to set just hit enter and it will give generate one wallet for us, and in return, it will tell where our private key is stored and share the public key and passphrase with us.

### creating a token
spl-token create-token

### create a account for token
spl-token create-account TOKEN_ADDRESS

TOKEN_ADDRESS: the address received while creating token.

Note: An account holds token.