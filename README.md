
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
# Update contractAddress in mint-nft.js for new ropsten contract address
# e.g. const contractAddress = "0xA61d5349B2DD0DE7aD48291008CEA6Ca109CD6d7"

```

3. mint
```
#modify pinata if you want to upload new image
#hash P01:wahxlnzsbhpzqwggku@mrvpm.net#VV2g45DyfY44:frsgkcotlbsaqnitef@pptrvv.com
node scripts/mint-nft.js
```
