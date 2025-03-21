# Welcome to BNB Chain Knowledge Base
[
  {
    "type": "function",
    "name": "BC_FUSION_CHANNELID",
    "inputs": [],
    "outputs": [
      {
        "name": "",
        "type": "uint8",
        "internalType": "uint8"
      }
    ],
    "stateMutability": "view"
  },
  {
    "type": "function",
    "name": "SOURCE_CHAIN_ID",
    "inputs": [],
    "outputs": [
      {
        "name": "",
        "type": "string",
        "internalType": "string"
      }
    ],
    "stateMutability": "view"
  },
  {
    "type": "function",
    "name": "STAKING_CHANNELID",
    "inputs": [],
    "outputs": [
      {
        "name": "",
        "type": "uint8",
        "internalType": "uint8"
      }
    ],
    "stateMutability": "view"
  },
  {
    "type": "function",
    "name": "addToBlackList",
    "inputs": [
      {
        "name": "account",
        "type": "address",
        "internalType": "address"
      }
    ],
    "outputs": [],
    "stateMutability": "nonpayable"
  },
  {
    "type": "function",
    "name": "approvalAddress",
    "inputs": [],
    "outputs": [
      {
        "name": "",
        "type": "address",
        "internalType": "address"
      }
    ],
    "stateMutability": "view"
  },
  {
    "type": "function",
    "name": "blackList",
    "inputs": [
      {
        "name": "",
        "type": "address",
        "internalType": "address"
      }
    ],
    "outputs": [
      {
        "name": "",
        "type": "bool",
        "internalType": "bool"
      }
    ],
    "stateMutability": "view"
  },
  {
    "type": "function",
    "name": "cancelTokenRecover",
    "inputs": [
      {
        "name": "tokenSymbol",
        "type": "bytes32",
        "internalType": "bytes32"
      },
      {
        "name": "attacker",
        "type": "address",
        "internalType": "address"
      }
    ],
    "outputs": [],
    "stateMutability": "nonpayable"
  },
  {
    "type": "function",
    "name": "initialize",
    "inputs": [],
    "outputs": [],
    "stateMutability": "nonpayable"
  },
  {
    "type": "function",
    "name": "isPaused",
    "inputs": [],
    "outputs": [
      {
        "name": "",
        "type": "bool",
        "internalType": "bool"
      }
    ],
    "stateMutability": "view"
  },
  {
    "type": "function",
    "name": "isRecovered",
    "inputs": [
      {
        "name": "node",
        "type": "bytes32",
        "internalType": "bytes32"
      }
    ],
    "outputs": [
      {
        "name": "",
        "type": "bool",
        "internalType": "bool"
      }
    ],
    "stateMutability": "view"
  },
  {
    "type": "function",
    "name": "merkleRoot",
    "inputs": [],
    "outputs": [
      {
        "name": "",
        "type": "bytes32",
        "internalType": "bytes32"
      }
    ],
    "stateMutability": "view"
  },
  {
    "type": "function",
    "name": "merkleRootAlreadyInit",
    "inputs": [],
    "outputs": [
      {
        "name": "",
        "type": "bool",
        "internalType": "bool"
      }
    ],
    "stateMutability": "view"
  },
  {
    "type": "function",
    "name": "pause",
    "inputs": [],
    "outputs": [],
    "stateMutability": "nonpayable"
  },
  {
    "type": "function",
    "name": "recover",
    "inputs": [
      {
        "name": "tokenSymbol",
        "type": "bytes32",
        "internalType": "bytes32"
      },
      {
        "name": "amount",
        "type": "uint256",
        "internalType": "uint256"
      },
      {
        "name": "ownerPubKey",
        "type": "bytes",
        "internalType": "bytes"
      },
      {
        "name": "ownerSignature",
        "type": "bytes",
        "internalType": "bytes"
      },
      {
        "name": "approvalSignature",
        "type": "bytes",
        "internalType": "bytes"
      },
      {
        "name": "merkleProof",
        "type": "bytes32[]",
        "internalType": "bytes32[]"
      }
    ],
    "outputs": [],
    "stateMutability": "nonpayable"
  },
  {
    "type": "function",
    "name": "removeFromBlackList",
    "inputs": [
      {
        "name": "account",
        "type": "address",
        "internalType": "address"
      }
    ],
    "outputs": [],
    "stateMutability": "nonpayable"
  },
  {
    "type": "function",
    "name": "resume",
    "inputs": [],
    "outputs": [],
    "stateMutability": "nonpayable"
  },
  {
    "type": "function",
    "name": "updateParam",
    "inputs": [
      {
        "name": "key",
        "type": "string",
        "internalType": "string"
      },
      {
        "name": "value",
        "type": "bytes",
        "internalType": "bytes"
      }
    ],
    "outputs": [],
    "stateMutability": "nonpayable"
  },
  {
    "type": "event",
    "name": "BlackListed",
    "inputs": [
      {
        "name": "target",
        "type": "address",
        "indexed": true,
        "internalType": "address"
      }
    ],
    "anonymous": false
  },
  {
    "type": "event",
    "name": "Initialized",
    "inputs": [
      {
        "name": "version",
        "type": "uint8",
        "indexed": false,
        "internalType": "uint8"
      }
    ],
    "anonymous": false
  },
  {
    "type": "event",
    "name": "ParamChange",
    "inputs": [
      {
        "name": "key",
        "type": "string",
        "indexed": false,
        "internalType": "string"
      },
      {
        "name": "value",
        "type": "bytes",
        "indexed": false,
        "internalType": "bytes"
      }
    ],
    "anonymous": false
  },
  {
    "type": "event",
    "name": "Paused",
    "inputs": [],
    "anonymous": false
  },
  {
    "type": "event",
    "name": "ProtectorChanged",
    "inputs": [
      {
        "name": "oldProtector",
        "type": "address",
        "indexed": true,
        "internalType": "address"
      },
      {
        "name": "newProtector",
        "type": "address",
        "indexed": true,
        "internalType": "address"
      }
    ],
    "anonymous": false
  },
  {
    "type": "event",
    "name": "Resumed",
    "inputs": [],
    "anonymous": false
  },
  {
    "type": "event",
    "name": "TokenRecoverRequested",
    "inputs": [
      {
        "name": "ownerAddress",
        "type": "bytes",
        "indexed": false,
        "internalType": "bytes"
      },
      {
        "name": "tokenSymbol",
        "type": "bytes32",
        "indexed": false,
        "internalType": "bytes32"
      },
      {
        "name": "account",
        "type": "address",
        "indexed": false,
        "internalType": "address"
      },
      {
        "name": "amount",
        "type": "uint256",
        "indexed": false,
        "internalType": "uint256"
      }
    ],
    "anonymous": false
  },
  {
    "type": "event",
    "name": "UnBlackListed",
    "inputs": [
      {
        "name": "target",
        "type": "address",
        "indexed": true,
        "internalType": "address"
      }
    ],
    "anonymous": false
  },
  {
    "type": "error",
    "name": "AlreadyPaused",
    "inputs": []
  },
  {
    "type": "error",
    "name": "AlreadyRecovered",
    "inputs": []
  },
  {
    "type": "error",
    "name": "ApprovalAddressNotInitialized",
    "inputs": []
  },
  {
    "type": "error",
    "name": "InBlackList",
    "inputs": []
  },
  {
    "type": "error",
    "name": "InvalidApprovalSignature",
    "inputs": []
  },
  {
    "type": "error",
    "name": "InvalidOwnerPubKeyLength",
    "inputs": []
  },
  {
    "type": "error",
    "name": "InvalidOwnerSignatureLength",
    "inputs": []
  },
  {
    "type": "error",
    "name": "InvalidProof",
    "inputs": []
  },
  {
    "type": "error",
    "name": "InvalidValue",
    "inputs": [
      {
        "name": "key",
        "type": "string",
        "internalType": "string"
      },
      {
        "name": "value",
        "type": "bytes",
        "internalType": "bytes"
      }
    ]
  },
  {
    "type": "error",
    "name": "MerkleRootAlreadyInitiated",
    "inputs": []
  },
  {
    "type": "error",
    "name": "MerkleRootNotInitialized",
    "inputs": []
  },
  {
    "type": "error",
    "name": "NotPaused",
    "inputs": []
  },
  {
    "type": "error",
    "name": "OnlyCoinbase",
    "inputs": []
  },
  {
    "type": "error",
    "name": "OnlyProtector",
    "inputs": []
  },
  {
    "type": "error",
    "name": "OnlySystemContract",
    "inputs": [
      {
        "name": "systemContract",
        "type": "address",
        "internalType": "address"
      }
    ]
  },
  {
    "type": "error",
    "name": "OnlyZeroGasPrice",
    "inputs": []
  },
  {
    "type": "error",
    "name": "TokenRecoverPortalPaused",
    "inputs": []
  },
  {
    "type": "error",
    "name": "UnknownParam",
    "inputs": [
      {
        "name": "key",
        "type": "string",
        "internalType": "string"
      },
      {
        "name": "value",
        "type": "bytes",
        "internalType": "bytes"
      }
    ]
  }
]

This is the BNB Chain Knowledge Base documentation for the BNB Chain developers. It is based on the Mkdocs Material theme. 

## Prerequisite  

* `pip install mkdocs-material` - install mkdocs-material.
* `pip install mkdocs-video` - install mkdocs-video.
* `pip install mkdocs-redirects` - install mkdocs-redirects plugin.

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

## 📜 License

Copyright (c) 2024 BNB Chain 

