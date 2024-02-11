# Blockchain Web Application
![image](https://github.com/TakudzwaChoto/Blockcahin-Application/assets/56199912/81c2968a-d450-46f7-b6c8-eb171c817177)


Created a single web page application to allow users to create a wallet that creates, loads and holds private and public keys. This helps to manage transaction signing and verification. 
As new blocks are mined, users are rewarded with money and new blocks get added to a blockchain data structure. Users are allowed to engage in transactions to send money to recipients, Transactions are broadcasted from sender to receiver upon completing successfully. 

 ## Getting Started
 These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.
 
## Prequisites
### Python 3.11.0 or + Needs to be installed


## Installation 
```
 On Windows:
    python -m pip install flask
    python -m pip install flask_cors
    python -m pip install requests
 ```
### After installing the above packages, please open up node.py to view where code execution starts. 
```python
if __name__ == '__main__':
    from argparse import ArgumentParser
    parser = ArgumentParser()
    parser.add_argument('-p', '--port', type=int, default=5000)
    args = parser.parse_args()
    port = args.port
    wallet = Wallet(port)
    blockchain = Blockchain(wallet.public_key, port)
    print("Starting Server")
    app.run(host='0.0.0.0', port=port)
    print("Server Started")
```

### Running the following command will get web service running on port 5000
```
    python node.py
```
Can run web service on different port by running the following command:
```
   python node.py --port <Port Number> 
```

## Technology Stack
* Python (backend)
* Flask Web Framework (backend to handle RESTFul routes)
* HTML (frontend)
* CSS (frontend)
* VueJS(frontend)

## Authors

* **Takudzwa Choto**
                                                                                                                                           
                                                                                                                         contact me at: ctakudzwa95@gmail.com

![image](https://github.com/TakudzwaChoto/Blockcahin-Application/assets/56199912/66b2800d-0a9b-4f3a-b95d-7211bcfdee7a)



