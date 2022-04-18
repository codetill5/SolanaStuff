### How to create collection.

### Preparing Assets and Metadata

Here is the sample metadata.

{
"name": "Battlefield",
"symbol": "BF",
"description": "Collection of 5 on the blockchain. This is the number 1/5.",
"seller_fee_basis_points": 500,
"image": "0.jpg",
"attributes": [
{ "trait_type": "Layer-1", "value": "0" },
{ "trait_type": "Layer-2", "value": "0" },
{ "trait_type": "Layer-3", "value": "0" },
{ "trait_type": "Layer-4", "value": "1" }
],
"properties": {
"creators": [
{ "address": "8iVFCjBobfQnYzS4wAxx5j1jVyixmQ79uF6G1kRkAPTA", "share": 100 }
],
"files": [{ "uri": "0.jpg", "type": "image/jpg" }]
},
"collection": { "name": "numbers", "family": "numbers" }
}

**properties.creators.share** : Means share they get of royalties.
**seller_fee_basis_points** : This is your royalties. 500 here means 5% of after market sales or secondary market sales,
payout to this address in royalties,



Errors:
 C:\Users\root\Documents\metaplex> npx ts-node js/packages/cli/src/candy-machine-v2-cli.ts --version

 PubKey: 8iVFCjBobfQnYzS4wAxx5j1jVyixmQ79uF6G1kRkAPTA

 solana config set keypair <file_path_file_system_wallet>

solana-keypair -o mywal.json
 solana config set --keypair C:\Users\root\Documents\metaplex\js\my-wal.json

 ----

 npx ts-node js/packages/cli/src/candy-machine-v2-cli.ts upload \
    -e devnet \
    -k my-wal.json \
    -cp config.json \
    -c example \
    ./assets-pictures


npx ts-node js/packages/cli/src/candy-machine-v2-cli.ts upload  -e devnet  -k my-wal.json  -cp config.json -c example ./assets-pictures



npx ts-node js/packages/cli/src/candy-machine-v2-cli.ts verify_upload -e devnet -k js\my-wal.json -c example


pubKey: B1a114xHsNi3TDMKKZTwAM5nv31SjWfs1GBWmnBDUvBy
CANDYMACHINEKEY: mR1eGqmHLddAEPhAbaoPCoUw9So2Yac7d6ZCVMEtiZK