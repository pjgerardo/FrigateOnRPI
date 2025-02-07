Install Frigate on Rasberry Pi 3 running Ubuntu Core
docker run -d --name frigate --restart=unless-stopped --device /dev/video11 --shm-size=64m   -v frigate_volume:/media/frigate   -v frigate_volume:/config -v /etc/localtime:/etc/localtime:ro -e FRIGATE_RTSP_PASSWORD='yourpassword' -p 8971:8971 -p 8554:8554 -p 8555:8555/tcp -p 8555:8555/udp ghcr.io/blakeblackshear/frigate:stable
