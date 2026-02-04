docker compose up -d --scale counting=3 --scale dashboard=3
docker network ls
docker network inspect consul-cicd-demo_appnet
sleep 12 && docker logs consul-cicd-demo-registrator-1