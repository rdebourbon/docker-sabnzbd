# docker sabnzbd
This is a Dockerfile to set up "SABnzbd" - (http://sabnzbd.org/)
Build from docker file
```
git clone https://github.com/rdebourbon/docker-sabnzbd.git
cd docker-sabnzbd
docker build -t sabnzbd .
```
docker run -d -h *your_host_name* --restart-always -v /*your_config_location*:/volumes/config -v /*your_videos_location*:/volumes/media -p 8080:8080 -p 9090:9090 sabnzbd
