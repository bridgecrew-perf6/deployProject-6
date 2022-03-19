# Udagram

This application was provided by Udacity, as a starter project for the Udacity's Javascript nanodegree course. Udagram is an application whose purpose is to allow users to create posts and share with other people.

## Getting Started

### To view a live demo:
1- Full working application:
http://udagram-bucket-thegux.s3-website-us-east-1.amazonaws.com/

2- API:
http://udagram-api-thegux-dev.us-east-1.elasticbeanstalk.com/api/v0

### To run this project on your own
To get started, first notice that both the frontend and backend are located in this repository. To build this project properly, you must:

1. Make sure you have Node (>= @14.15.1 version), npm (>= @6.14.8), Angular CLI, AWS CLI v2 and Eb CLI installed.
2. Create an environment using AWS Eb and associate the udagram-api with it (Please, remember to initiate elastic beanstalk using eb init)
3. Configure and RDS for running the database and an S3 bucket 
4. Configure a bucket for hosting post pictures
5. Update your deploy.sh with your bucket name
6. Setup environmemt variables listed at the ENV Variables section of this readme in your CI and also in your EBS.
7. Commit your project and wait for the pipeline to finish. Then, access your bucket's URL.

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
2. `npm run test`
3. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Service Health Status

### Elastic Beanstalk
<img width="654" alt="image" src="https://user-images.githubusercontent.com/60764149/159109410-cab685cc-ac98-4c74-a3b7-78a5ea414fca.png">

### RDS
<img width="873" alt="image" src="https://user-images.githubusercontent.com/60764149/159109524-58fbd916-ce20-4a1b-8e64-0b7fcda0811b.png">

### S3 (though public, stable and healthy)
<img width="861" alt="image" src="https://user-images.githubusercontent.com/60764149/159109555-3840406c-ec7d-4f8d-a758-28b1de6b20ff.png">

### CIRLECI
<img width="425" alt="image" src="https://user-images.githubusercontent.com/60764149/159109594-82736b55-199e-44c6-b87a-44cce592eb5a.png">
<img width="798" alt="image" src="https://user-images.githubusercontent.com/60764149/159111795-80291643-b1d7-4da3-ad01-9bf5850d663f.png">




## Infrastructure Overview Diagram
![UDAGRAM'S INFRASTRUCTURE OVERVIEW](https://user-images.githubusercontent.com/60764149/159110432-b6450ba3-9b14-4e34-957e-6e9ab11b324f.jpeg)

## Pipeline's Overview Diagram
![AWS (2019) horizontal framework](https://user-images.githubusercontent.com/60764149/159111993-8b97c3cc-85bf-4516-9b1c-2c7d8ee78764.jpeg)


## Environment variables
- POSTGRES_USERNAME
- POSTGRES_PASSWORD
- POSTGRES_DBPOSTGRES_DB
- PORT
- POSTGRES_HOST
- AWS_REGION
- AWS_PROFILE
- AWS_BUCKET
- AWS_ACCESS_KEY
- URL
- JWT_SECRET

Configure these on your CI/CD platform:
- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## License

[License](LICENSE.txt)
