# Ethereum genesis block JSON file

# Problem 
Sometimes, we mistakenly do 
$ someGeth init somePrivateGenesis.json

then your ~/Library/Ethereum (defaut mainnet datadir in OSX case) genesis block information has been changed.

So you can not use ~/Library/Ethereum for mainnet

# How we can fix
$ someGeth --datadir ~/Library/Ethereum init genesis_frontier.json 

then your ~/Library/Ethereum can be used again for mainnet. (But needs to wait for finish of reading states).
