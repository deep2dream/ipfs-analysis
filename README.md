# ipfs-analysis
ipfs, filecoin, ...
#### all in one
- https://github.com/ipfs/awesome-ipfs
#### file-video
- https://github.com/livepeer/file-video
- https://github.com/livepeer/file-video/blob/master/.env.local.example
- https://vercel.com/deep2dream/file-video
```
```
#### [lotus + ipfs +ethereum](https://github.com/truffle-box/filecoin-box)
*ganche works with node.js 12.13.1. It doesn't go well with 16.x.x*
```
$ nvm use 12.13.1
$ node --version
>>>
v12.13.1

$ npm install -g truffle
$ npm i truffle-plugin-debugger

$ mkdir filecoin & cd filecoin
$ truffle unbox filecoin

[run.filecoin.rpc]
filecoin $ npx ganache filecoin

[run.filecoin.browser]
$ git clone https://github.com/trufflesuite/filecoin-network-inspector
filecoin-network-inspector$ git checkout ganache-changes
filecoin-network-inspector$ npm install
filecoin-network-inspector$ npm run start

[run.ethereum.rpc]
filecoin $ npx ganache ethereum

[test]
curl -X POST \
     -H 'Content-Type: application/json' \
     -d '{"jsonrpc":"2.0","id":0,"method":"Filecoin.ClientStartDeal","params":[{"Data":{"TransferType":"graphsync","Root":{"/":"QmZTR5bcpQD7cFgTorqxZDYaew1Wqgfbd2ud9QqGPAkK2V"},"PieceCid":null,"PieceSize":0},"Wallet":"t3s3la37547tijmoeiep7ktogws3tep2eqrralh7rhi2mpe46q574gceyy467356onblzvwf7ejlelo2rdsg4q","Miner":"t01000","EpochPrice":"2500","MinBlocksDuration":300}]}' \
     http://localhost:7777/rpc/v0

```
