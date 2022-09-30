## Setup docker and jenkins

Create `.yaml` file to setup docker and jenkins using ansible playbook

![Screenshot from 2022-09-30 01-47-17](https://user-images.githubusercontent.com/56712612/193117076-c253b08b-b7fa-40ed-b766-7ad38fe5872a.png)

![Screenshot from 2022-09-30 01-47-27](https://user-images.githubusercontent.com/56712612/193117087-df7d8f9d-00db-481c-98b2-4589ec8538fe.png)

![Screenshot from 2022-09-30 01-47-35](https://user-images.githubusercontent.com/56712612/193117099-964b60c7-0cf8-4f84-926b-87f998a35a49.png)

Run ansible-playbook

![Screenshot from 2022-09-30 01-51-07](https://user-images.githubusercontent.com/56712612/193117716-ce6cb2a1-785c-4129-b9ac-dd70ff47e36a.png)

Run command `docker logs jenkins` in the server and copy the password to unlock jenkins

![Screenshot from 2022-09-30 01-51-55](https://user-images.githubusercontent.com/56712612/193118017-ce58e690-2bc7-405a-8442-1a89eb4d3a59.png)

Open jenkins url and insert the password

![Screenshot from 2022-09-30 01-55-24](https://user-images.githubusercontent.com/56712612/193118649-a32e00ae-693e-4b1d-bc29-626ba1556cc3.png)

Select suggestion plugin

![Screenshot from 2022-09-30 01-56-44](https://user-images.githubusercontent.com/56712612/193118972-4aa0e4cf-e669-4b84-b829-5b32a55f1788.png)

Create admin user

![Screenshot from 2022-09-30 02-14-53](https://user-images.githubusercontent.com/56712612/193122248-1fd95021-cb8a-4f0d-8b43-ab1d4315f472.png)

Insert URL

![Screenshot from 2022-09-30 02-15-50](https://user-images.githubusercontent.com/56712612/193122453-4ceca953-4298-4a21-8a37-e23d575a7964.png)

Select manage jenkins > available plugins, and search for ssh

![Screenshot from 2022-09-30 02-16-41](https://user-images.githubusercontent.com/56712612/193123049-20f9ae3c-e46f-4459-88d1-d252d655d02c.png)

![Screenshot from 2022-09-30 02-17-59](https://user-images.githubusercontent.com/56712612/193123055-0eb23824-450c-4ab4-a4c1-16b961f36177.png)

Select manage jenkins > manage credentials > click system > add domain

![Screenshot from 2022-09-30 02-16-41](https://user-images.githubusercontent.com/56712612/193123627-4556420b-441c-47b9-882c-c7cafc714332.png)

![Screenshot from 2022-09-30 02-20-38](https://user-images.githubusercontent.com/56712612/193123633-d0bcdb3c-074f-40b7-a822-37d2ee34e6f8.png)

add new domain and save

![Screenshot from 2022-09-30 02-24-57](https://user-images.githubusercontent.com/56712612/193124071-89b0d2d6-0898-4106-bdf7-e6b9e5a5dedd.png)

after create new domain, click add credentials

![Screenshot from 2022-09-30 02-25-56](https://user-images.githubusercontent.com/56712612/193124281-d899272f-034c-4d82-b085-a6b5de3c5cb2.png)

![Screenshot from 2022-09-30 02-29-27](https://user-images.githubusercontent.com/56712612/193124860-53a7ac7f-86a4-4dd1-9b8e-8e82eb5d720a.png)

![Screenshot from 2022-09-30 02-29-44](https://user-images.githubusercontent.com/56712612/193124864-c43e43eb-e9a7-4081-abd0-c75f87a06c3c.png)

## Frontend pipeline

Create `Jenkinsfile` inside the repo

![Screenshot from 2022-09-30 06-49-16](https://user-images.githubusercontent.com/56712612/193161397-9fd602f3-4031-4c87-9ebf-fbb73ac6cc17.png)

![Screenshot from 2022-09-30 06-49-32](https://user-images.githubusercontent.com/56712612/193161403-eeaa6c45-9959-407a-a05d-c8327664aa51.png)

![Screenshot from 2022-09-30 06-49-41](https://user-images.githubusercontent.com/56712612/193161408-a3080e54-e642-419b-98a5-c2e742d5cd4d.png)

Create a new pipeline in Jenkins

![Screenshot from 2022-09-30 06-50-34](https://user-images.githubusercontent.com/56712612/193161549-e3e157dd-7ed0-492f-b69a-91ffd20485ab.png)

![Screenshot from 2022-09-30 06-54-36](https://user-images.githubusercontent.com/56712612/193161991-a1938e9e-cfc8-44f7-8a9e-164652ad75e2.png)

![Screenshot from 2022-09-30 06-54-49](https://user-images.githubusercontent.com/56712612/193161996-0cf490a4-aae7-4f13-94c3-8f991941332c.png)

![Screenshot from 2022-09-30 06-55-01](https://user-images.githubusercontent.com/56712612/193162005-f45e5f5d-b745-4fbf-b895-821901d5058c.png)

![Screenshot from 2022-09-30 06-55-23](https://user-images.githubusercontent.com/56712612/193162013-71794ca7-829e-40ae-ad25-6223aee635ba.png)

![Screenshot from 2022-09-30 06-55-31](https://user-images.githubusercontent.com/56712612/193162019-ef8a3a72-d006-4712-bbf0-41d4f9cd28d5.png)

Add github webhook

![Screenshot from 2022-09-30 07-01-00](https://user-images.githubusercontent.com/56712612/193162488-5058d196-be2d-4dec-a362-960dc0e912eb.png)

## Backend pipeline

Create `Jenkinsfile` inside the repo

![Screenshot from 2022-09-30 07-05-33](https://user-images.githubusercontent.com/56712612/193162850-f72b5aba-c162-4e8b-b921-2c1acffa880b.png)

![Screenshot from 2022-09-30 07-05-45](https://user-images.githubusercontent.com/56712612/193162859-6b5168c1-5d76-4cd4-8780-51d31661fa6c.png)

![Screenshot from 2022-09-30 07-05-54](https://user-images.githubusercontent.com/56712612/193162864-3c9b92f4-9773-45b3-8528-4bc7579cf994.png)

Create a new pipeline in Jenkins

![Screenshot from 2022-09-30 07-07-06](https://user-images.githubusercontent.com/56712612/193162971-43e6a4c6-8df8-46c9-ad03-c3ec32bb1ee2.png)

![Screenshot from 2022-09-30 07-08-53](https://user-images.githubusercontent.com/56712612/193163130-4b66fa71-1926-4154-94e0-51846e45e19e.png)

![Screenshot from 2022-09-30 07-09-01](https://user-images.githubusercontent.com/56712612/193163134-5b195b4f-9057-4f47-bebd-d23544251d8b.png)

![Screenshot from 2022-09-30 07-09-11](https://user-images.githubusercontent.com/56712612/193163141-019cba5c-b375-4c06-926f-bdbdfbc9f648.png)

![Screenshot from 2022-09-30 07-09-23](https://user-images.githubusercontent.com/56712612/193163143-8f754a25-8ffb-4644-8ff0-7093d6265862.png)

![Screenshot from 2022-09-30 07-09-28](https://user-images.githubusercontent.com/56712612/193163148-3f24e141-406a-44e6-9348-87650da92f0a.png)

Add github webhook

![Screenshot from 2022-09-30 07-14-20](https://user-images.githubusercontent.com/56712612/193163564-fbaf40d4-5875-41bb-90db-3e1bbda957dc.png)

