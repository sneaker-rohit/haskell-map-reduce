For the requirements of CS7050 Course. The project uses the master slave communication pattern of cloud haskell and pushes out the work (i.e, to count the word frequency) to the slave nodes. We run it first locally on just one node and then distribute this task onto several slave nodes.

## Getting started with executing this project
```
stack setup
stack build
```

## Run the project on single node (locally)
```
stack exec mapreduce-haskell-project local count data
```
## Run the project in a distributed fashion using Docker
```
stack image container 
docker-compose up
stack exec mapreduce-haskell-project master localhost 8080 count 4300.txt
```

