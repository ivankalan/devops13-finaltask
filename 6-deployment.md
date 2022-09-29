## Prerequisite

Clone the app

![Screenshot from 2022-09-29 17-02-13](https://user-images.githubusercontent.com/56712612/193008539-01908c24-a870-4fb3-b0e9-cdc60b4fc577.png)

Move to the production branch, do this in both repos

![Screenshot from 2022-09-29 17-32-56](https://user-images.githubusercontent.com/56712612/193009055-91a4bf29-cad9-4ae0-9fbd-90d80ced1430.png)

Copy the contents of the .gitignore to the .dockerignore

![Screenshot from 2022-09-29 17-40-45](https://user-images.githubusercontent.com/56712612/193010664-9ba45bfd-d660-4fd6-977a-11ea8c036889.png)

Login to docker

![Screenshot from 2022-09-29 17-41-51](https://user-images.githubusercontent.com/56712612/193010871-ea81807e-269f-435a-89c5-1290c0ad3f37.png)

## Backend deployment

Create `Dockerfile` in folder `literature-backend`

![Screenshot from 2022-09-29 17-46-58](https://user-images.githubusercontent.com/56712612/193011972-875b4667-2c15-40a4-9bc9-f8ee0951bf9f.png)

Build docker image

![Screenshot from 2022-09-29 18-01-54](https://user-images.githubusercontent.com/56712612/193014863-146a5ded-21ae-4d7f-84f3-b7a51385e395.png)

Create `docker-compose.yml`

![Screenshot from 2022-09-29 20-10-01](https://user-images.githubusercontent.com/56712612/193040187-9cc935b9-79be-4d0e-abef-c743f74c3052.png)

Run docker compose

![Screenshot from 2022-09-29 20-11-10](https://user-images.githubusercontent.com/56712612/193040450-ada478e5-87e4-46e3-b355-287d5ebbe23b.png)

## Frontend deployment

Open file `config.js` in the `src/config/config.js` and edit the baseURL to your publicly accesable url

![Screenshot from 2022-09-29 22-53-36](https://user-images.githubusercontent.com/56712612/193079941-ba7dad56-e429-4739-a058-702be809794e.png)

Open `.dockerignore` and comment line `/build`

![Screenshot from 2022-09-29 22-56-31](https://user-images.githubusercontent.com/56712612/193080253-13bdce5c-5bba-49ed-908b-439a4f1c6bdd.png)

Install npm using nvm

![Screenshot from 2022-09-29 22-57-26](https://user-images.githubusercontent.com/56712612/193080498-42dbe541-3c65-4539-a85b-3796e8fb8f4a.png)

Run command `npm install` and `npm run build`

![Screenshot from 2022-09-29 23-00-10](https://user-images.githubusercontent.com/56712612/193081119-7448936c-1da9-4295-93e7-49b8888c000a.png)

Create `Dockerfile`

![Screenshot from 2022-09-29 23-03-06](https://user-images.githubusercontent.com/56712612/193081640-64785dd7-d01f-47ea-85f8-fed5ad951b01.png)

Build docker image

![Screenshot from 2022-09-29 23-11-13](https://user-images.githubusercontent.com/56712612/193083425-1b1a9eaf-bcc6-41ec-8c18-8e6cd83b316a.png)

Create docker compose file

![Screenshot from 2022-09-29 23-11-59](https://user-images.githubusercontent.com/56712612/193083553-76763669-725f-45ca-b61e-990d596b10fd.png)

Run docker compose

![Screenshot from 2022-09-29 23-14-51](https://user-images.githubusercontent.com/56712612/193084140-75a94696-6974-4e59-b49a-598b0a65c28b.png)








