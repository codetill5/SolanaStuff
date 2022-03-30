# HOOKS

useUserArts() // will get all nft metadata 

###  Get Wallet Address

import { useWallet } from '@solana/wallet-adapter-react';
const wallet = useWallet();
wallet.publicKey?.toBase58() 