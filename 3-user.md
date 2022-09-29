## Create user and enable login without password

Create ansible-playbook file and write configuration like this

![1  type the configuration file like this fix](https://user-images.githubusercontent.com/56712612/192981244-a189e4ed-6a12-4c27-b08a-d55447506e2c.png)

![4  add config to user yaml for sign in without password and run ansible-playbook](https://user-images.githubusercontent.com/56712612/192981533-b619354d-2467-4bf4-9c48-a288e8d6c626.png)

Create encrypted password using command `mkpasswd --method=sha512`

![2  create encrypted password](https://user-images.githubusercontent.com/56712612/192981590-d42c8da0-af34-4ff5-9d80-bc67420e4fed.png)

Run ansible-playbook

![3  run ansible-playbook](https://user-images.githubusercontent.com/56712612/192981939-02fc093d-38bf-4c73-ae55-1db89ffbfb95.png)

Try to login to the server

![5  try to login to the server](https://user-images.githubusercontent.com/56712612/192981984-9cae2ead-dab0-44dc-80f5-b8fef2e899ff.png)
