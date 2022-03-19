# Pipeline Documentation
The pipeline was constructed using Circle CI. It consists of simple steps, such as: installing dependencies, building steps and deployment steps. To view all of the mentioned steps, please check the images listed below.

## Environment variables
Please Configure the following environment variables in your circle CI project:

- POSTGRES_USERNAME
- POSTGRES_PASSWORD
- POSTGRES_DBPOSTGRES_DB
- PORT
- POSTGRES_HOST
- AWS_REGION
- AWS_PROFILE
- AWS_BUCKET
- URL
- JWT_SECRET
- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY
- AWS_ACCESS_KEY
- AWS_REGION
- 
### Environment Config Screenshot
<img width="491" alt="image" src="https://user-images.githubusercontent.com/60764149/159126007-65ae8311-104c-4d85-99a2-ba15e32ae121.png">

## CIRLECI
<img width="521" alt="image" src="https://user-images.githubusercontent.com/60764149/159125964-197cdd25-4b60-4f05-8bcc-69bf333e082c.png">
<img width="659" alt="image" src="https://user-images.githubusercontent.com/60764149/159125865-eb97d9bb-88ae-4285-a240-3b0f33ac0fff.png">


### Pipeline's Overview Diagram
![AWS (2019) horizontal framework](https://user-images.githubusercontent.com/60764149/159111993-8b97c3cc-85bf-4516-9b1c-2c7d8ee78764.jpeg)


#### Pipeline note
Please note that only changes applied to master will be deployed.
<img width="648" alt="image" src="https://user-images.githubusercontent.com/60764149/159121589-3f1f5e71-9948-4bfe-b550-0dbf834c8b8d.png">
