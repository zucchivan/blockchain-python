# blockchain-python

Simple blockchain built for learning purposes following @dvf guidelines on [Building a Blockchain](https://medium.com/p/117428612f46).

The services are exposed via REST using Flask.

## Installation

1. Make sure [Python 3.6+](https://www.python.org/downloads/) is installed. 
2. Install [pipenv](https://github.com/kennethreitz/pipenv). 

```
$ pip install pipenv 
```
3. Install requirements  
```
$ pipenv install 
``` 

4. Run the server:
    * `$ pipenv run python blockchain.py` 
    * `$ pipenv run python blockchain.py -p 5001`
    * `$ pipenv run python blockchain.py --port 5002`
    
## Services

1. */mine*

GET endpoint that tells the server to mine a new block

2. */transactions/new*

POST endpoint that creates a new transaction to a block

3. */transactions/new*

GET endpoint that returns the full chain

4. */nodes/register*

POST endpoint that accepts a list of new nodes in the form of URLs.

5. */nodes/resolve* 

GET endpoint that runs the chain's Consensus Algorithm to resolve conflicts and ensure a node has the correct chain.
