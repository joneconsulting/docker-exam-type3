### Mac OS (Apple chip)
##### Docker Host 1 (for Manager)
* Host PC에서 실행
```
docker run --privileged --name manager -itd -p 10022:22 -p 8081:8080 -e container=docker -v /sys/fs/cgroup:/sys/fs/cgroup:rw --cgroupns=host edowon0623/docker-server:m1 /usr/sbin/init

docker exec -it manager bash
```
* Docker Container에서 실행 
```
systemctl start docker
```

##### Docker Host 2 (for Worker1)
* Host PC에서 실행
```
docker run --privileged --name worker1 -itd -p 20022:22 -p 8082:8080 -e container=docker -v /sys/fs/cgroup:/sys/fs/cgroup:rw --cgroupns=host edowon0623/docker-server:m1 /usr/sbin/init

docker exec -it worker1 bash
```
* Docker Container에서 실행 
```
systemctl start docker
```

##### Docker Host 3 (for Worker2)
* Host PC에서 실행
```
docker run --privileged --name worker2 -itd -p 30022:22 -p 8083:8080 -e container=docker -v /sys/fs/cgroup:/sys/fs/cgroup:rw --cgroupns=host edowon0623/docker-server:m1 /usr/sbin/init

docker exec -it worker2 bash
```
* Docker Container에서 실행 
```
systemctl start docker
```