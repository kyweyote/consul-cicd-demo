docker compose up -d --scale counting=3 --scale dashboard=3
docker network ls
docker network inspect consul-cicd-demo_appnet
sleep 12 && docker logs consul-cicd-demo-registrator-1

docker exec -it consul-cicd-demo-counting-1 /bin/sh
docker logs -f consul-cicd-demo-dnsmasq-1

docker exec -it consul-cicd-demo-dnsmasq-1 sh
cat /etc/dnsmasq.conf

docker exec -it consul-cicd-demo-counting-1 nslookup www.google.com 172.18.0.101