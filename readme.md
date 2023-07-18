# My Home Assistant Docker Compose

docker run -d \
  --name homeassistant \
  --privileged \
  --restart=unless-stopped \
  -e TZ=America/Sao_Paulo \
  -v /home/docker:/config \
  --network=host \
  ghcr.io/home-assistant/home-assistant:stable
  
  

/PATH_TO_YOUR_CONFIG points at the folder where you want to store your configuration and run it.

MY_TIME_ZONE is a tz database name, like TZ=America/Los_Angeles.

docker restart homeassistant


## Mosquitto


>  The default user is admin/password.