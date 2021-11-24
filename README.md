
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
```
