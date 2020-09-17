# swarm

1. `docker swarm init --advertise-addr <ip>`
2. paste the `docker swarm join ...` on additional "machines"
3. deploy portainer
  - `curl -L https://downloads.portainer.io/portainer-agent-stack.yml -o portainer-agent-stack.yml && docker stack deploy --compose-file=portainer-agent-stack.yml portainer`
4. click port 9000 to view
![port9k](./Capture.PNG)
