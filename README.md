
Goto: https://ethereum.org/en/developers/tutorials/how-to-write-and-deploy-an-nft/

1. Create scripts and npm install
```
curl -LSfs https://raw.githubusercontent.com/github167/demo-nft/simple-nft-ropsten/init.sh | sh
cd my-nft
```

2. compile
```
cat << EOF > .env
API_URL=https://eth-ropsten.alchemyapi.io/v2/-85Y6azzTCmhKOMo3ffwrl1MxyuSHOHN
PRIVATE_KEY=<<your private key>>
PUBLIC_KEY=<<your public key>>
EOF

npx hardhat compile
#npx hardhat run scripts/deploy.js --network ropsten
#Contract deployed to address: 0xA61d5349B2DD0DE7aD48291008CEA6Ca109CD6d7
#Contract deployed to address: 0x9E1752E5860F46c200081C40CB735D08CeE540f6
```
3. copy to pista

4. mint
```
#node scripts/mint-nft.js
```
