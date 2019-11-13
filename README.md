# privatechain

```
account : f032201151421de463860e1acfd79543085850f4
password : Sample
```

```
$ git clone git@github.com:Yosuke-Aramaki/sample-chain.git
$ cd sample-chain
$ geth --datadir node1/ --syncmode 'full' --port 30311 --rpc --rpcaddr '0.0.0.0' --rpcport 8545 --rpccorsdomain "*" --rpcvhosts "*" --rpcapi 'personal,db,eth,net,web3,txpool,miner' --ws --wsapi 'eth,web3,net' --wsorigins='*' --wsaddr='0.0.0.0' --wsport 8546 --networkid 1515 --gasprice '0'
```

```
$ cd sample-chain
$ geth attach ipc:node1/geth.ipc
> personal.unlockAccount(eth.coinbase,"sample",0)
> mimer.start()
```
