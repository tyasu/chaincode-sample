# chaincode-sample
My first chaincode for Hyperledger fabric. It can store only one key-value pairs.

##Deploy

```
{
  "jsonrpc": "2.0",
  "method": "deploy",
  "params": {
    "type": 1,
    "chaincodeID": {
      "name": "sample"
    },
    "ctorMsg": {
      "args": ["init", "hello"]
    }
  },
  "id": 1
}
```

##Invoke

```
{
  "jsonrpc": "2.0",
  "method": "invoke",
  "params": {
    "type": 1,
    "chaincodeID": {
      "name": "sample"
    },
    "ctorMsg": {
      "args": ["write", "This is my first chaincode"]
    }
  },
  "id": 3
}
```

##Query

```
{
  "jsonrpc": "2.0",
  "method": "query",
  "params": {
    "type": 1,
    "chaincodeID": {
      "name": "sample"
    },
    "ctorMsg": {
      "args": ["read", "key1"]
    }
  },
  "id": 3
}
```

