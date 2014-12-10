docker-cassandra-mesos-build
============================

Simple Dockerfile to build cassandra-mesos for CentOS 6.x


# Instruction
```sh
git clone https://github.com/sheepkiller/docker-cassandra-mesos-build.git
cd https://github.com/sheepkiller/docker-cassandra-mesos-build
git clone https://github.com/mesosphere/cassandra-mesos.git
chmod +x build.sh cassandra-mesos
cp -p build.sh cassandra-mesos
docker build -t tmp/build .
docker run -it --rm -v $(pwd)/cassandra-mesos:/build tmp/build
```

