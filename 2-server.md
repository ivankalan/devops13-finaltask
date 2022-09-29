## Create server using terraform

Create bash script to install terraform

![1  create bash script to install terraform](https://user-images.githubusercontent.com/56712612/192973022-eb7edd67-edb5-4bc5-974b-7b261a0c4bce.png)

Run bash script

![2  run bash script](https://user-images.githubusercontent.com/56712612/192973219-0e43f2bf-e67a-46ab-82e2-57bd2aac0d7e.png)

Check if terraform already installed

![3  check if terraform was installed](https://user-images.githubusercontent.com/56712612/192973385-414fd8f2-65d8-4a3e-aa98-210e7d7fddb8.png)

## Create vm in IDCH using terraform

Create a new folder and new file `.tf` to setup terraform configuration

![1  create config file for terraform to create a vm in IDCH](https://user-images.githubusercontent.com/56712612/192973610-7674e83a-5047-47ad-8ba8-c25c28ba618f.png)

Open terraform registry and search idcloudhost, click how to use this provider and copy the configuration

![3  scroll and click how to use this provider and copy the configuration](https://user-images.githubusercontent.com/56712612/192973867-97b99c18-f190-4a7a-ad5e-c059c6f18b1d.png)

Create configuration based on this picture

![4  create configuration like this](https://user-images.githubusercontent.com/56712612/192974410-363cac15-9a4b-4656-83b9-cb80fcb12196.png)

![5  and this](https://user-images.githubusercontent.com/56712612/192974418-23992f47-9a41-4d2a-a56d-fb99e047a1ac.png)

For the auth_token, fill this using idclouhost api token

![6  for the section auth token, fill this using idcloudhost api and setup like this](https://user-images.githubusercontent.com/56712612/192974614-f5e53f1e-ed0c-4311-8881-60f477737858.png)

To create idch api, click access at the side nav, and click new

![7  To create idch api, select access nav and click new the select the api, after created the api, will showing page like this and copy the api](https://user-images.githubusercontent.com/56712612/192975055-fdd12b90-21b8-420d-8a26-5a2fee244674.png)

And then create bash script to generate api token from idch api

![8  Then create config like this and fill the api token with api token was created before and fill the billing id with the user billing id in profile page](https://user-images.githubusercontent.com/56712612/192975726-94a70322-7dbd-4664-9bba-4bdbb34942ac.png)

Nb: don't forget to fill apikey using idch api key and billing_account_id with account id at the idch profile page

Run the bash script, and copy the token created by the script and paste it into the terraform configuration file

![9  Then run the bash script to create token auth and the result will be like this, copy the auth token and paste into config file](https://user-images.githubusercontent.com/56712612/192976197-0cbfc3b9-2be7-4eaa-8ad7-a2ba19816baf.png)

Run command `terraform init` to initialize terraform workdir

![10  run command terraform init to initialize the working directory of terraform](https://user-images.githubusercontent.com/56712612/192976740-a1e7084b-c4ba-4887-a280-42120778cc95.png)

Run the config by typing `terraform apply`

![11  then run the config with command terraform apply](https://user-images.githubusercontent.com/56712612/192976944-9ce296c4-17a9-433e-a5ee-69ee8441b76e.png)

type yes

![12  type yes, and wait for the terraform do the job](https://user-images.githubusercontent.com/56712612/192977006-5bb71a62-0fc1-4cbf-bed6-ca920f4384d5.png)

Terraform success

![13  if success, will show prompt like this, and then now check in the idch are the vm is created or not](https://user-images.githubusercontent.com/56712612/192977107-9e5cc020-17c3-4bf6-985b-27479889ee3b.png)

Check at the idch whether the vm has been created or not

![14  the result](https://user-images.githubusercontent.com/56712612/192977328-5deda78e-6714-46f4-a561-55ff42946611.png)

![15  the result 2](https://user-images.githubusercontent.com/56712612/192977367-488007d1-3bb4-4eec-b6ae-f559ffda7c5e.png)





