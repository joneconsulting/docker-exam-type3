1. Docker Swarm Init
* Manager에서 실행 
```
docker swarm init
```

2. Docker Swarm Join
* Worker1에서 실행 
```
docker swarm join --token SWMTKN-1-0fc40z7euidrshhtcr5mv2wyj391zc3wsdwybexjgcft8fn1d2-aumber64pj9yn0eqkfwtd9rdo 172.17.0.2:2377
```

* Worker2에서 실행
```
docker swarm join --token SWMTKN-1-0fc40z7euidrshhtcr5mv2wyj391zc3wsdwybexjgcft8fn1d2-aumber64pj9yn0eqkfwtd9rdo 172.17.0.2:2377
```

3. Docker Node 확인
* Worker2에서 실행
```
docker node ls
```