## Setup Docker and Postgresql docker image

Write configuration like this to install docker and setup postgresql

![1  create  yaml file and write config like this](https://user-images.githubusercontent.com/56712612/192993885-52a5d48b-f120-4183-b9e4-e66213092f70.png)

![2  like this too](https://user-images.githubusercontent.com/56712612/192994175-e9c15cb9-de47-41aa-9489-baebcd89eca0.png)

![3  and this](https://user-images.githubusercontent.com/56712612/192994186-775575cf-a465-45ac-a5c4-7d52f068d54b.png)

Run ansible-playbook

![4  and then run the ansible-playbook](https://user-images.githubusercontent.com/56712612/192994526-c76f32b0-a1a1-48ac-b875-bd55a06e3246.png)

Login to server and check if postgresql container is running

![5  login to the server and check if the postgresql docker image is running](https://user-images.githubusercontent.com/56712612/192994606-e0eba491-0b6a-44d1-a82a-e73fe73809fc.png)

## Create database

Login to server and enter the postgresql container and create `literature` database

![1  write the command like this](https://user-images.githubusercontent.com/56712612/192994903-91c2437b-5f3e-4abc-900a-76115553406d.png)

## Remote database

Login to another server and type command like this to remote database

![1  login to another server and write the command like this](https://user-images.githubusercontent.com/56712612/192995188-0a7ecf19-8dd9-4bbb-a347-7ba86db78769.png)
