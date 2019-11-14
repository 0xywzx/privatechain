# privatechain

```
account : 2b6920a024601760b1f287c7fec1c41e74d56d9c
password : Sample
```

```
$ git clone git@github.com:Yosuke-Aramaki/privatechain.git
$ cd sample-chain
$ geth --datadir node1/ --syncmode 'full' --port 30311 --rpc --rpcaddr '0.0.0.0' --rpcport 8545 --rpccorsdomain "*" --rpcvhosts "*" --rpcapi 'personal,db,eth,net,web3,txpool,miner' --ws --wsapi 'eth,web3,net' --wsorigins='*' --wsaddr='0.0.0.0' --wsport 8546 --networkid 1515 --gasprice '0'
```

```
$ cd sample-chain
$ geth attach ipc:node1/geth.ipc
> personal.unlockAccount(eth.coinbase,"Sample",0)
> mimer.start()
```
