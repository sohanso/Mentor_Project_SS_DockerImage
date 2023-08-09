# Mentor_Project_SS_DockerImage
Docker Image - Nginx with html file









sudo docker login -u sohanso
password - is access token
docker build -t ngi_mentor_img .(. is path of dockerfile)
docker tag ngi_mentor_img sohanso/ngi-mentor-proj
docker push sohanso/ngi-mentor-proj
#open new ec2 instace
sudo docker image pull sohanso/ngi-mentor-proj:latest
sudo docker run -d -p 80:80 --name mentor_app sohanso/ngi-mentor-proj

sudo docker stop <nameofcontainer>
sudo docker rm <nameofcontainer> 







docker image rm -f hello-world