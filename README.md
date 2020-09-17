# swarm

1. `docker swarm init --advertise-addr <ip>`
2. paste the `docker swarm join ...` on additional "machines"
3. deploy portainer
  - `curl -L https://downloads.portainer.io/portainer-agent-stack.yml -o portainer-agent-stack.yml && docker stack deploy --compose-file=portainer-agent-stack.yml portainer`
4. click port 9000 to view
![port9k](./Capture.PNG)
5. create a password
![pass](./Capture2.PNG)
6. view the visualizer
![viz1](./Capture4.PNG)
![viz2](./Capture5.PNG)
![viz3](./Capture6.PNG)
7. you now have a Docker Swarm cluster.
8. `git clone https://github.com/microservices-demo/microservices-demo && cd microservices-demo && docker-compose pull && docker stack deploy --compose-file deploy/docker-swarm/docker-compose.yml sockshop`
