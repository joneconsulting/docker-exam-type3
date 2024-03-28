### Mac OS (Apple chip)
##### Docker Host 1 (for Manager)
* Host PC에서 실행
```
docker exec -it manager bash
```
* Docker Container에서 실행 
```
systemctl start docker
```

##### Docker Host 2 (for Worker1)
* Host PC에서 실행
```
docker exec -it worker1 bash
```
* Docker Container에서 실행 
```
systemctl start docker
```

##### Docker Host 3 (for Worker2)
* Host PC에서 실행
```
docker exec -it worker2 bash
```
* Docker Container에서 실행 
```
systemctl start docker
```