# Infrastructure Description

The application is divided into two main folders: `udagram-api` for the backend and `udagram-frontend` for the frontend. Each folder contains its own configuration files including: `package.json`, `eslintrc.json`, and `.gitignore`.

## Technologies

There are various technologies used in the app, but the main ones are:

- **Backend:** `Node.js`, `Express`, `TypeScript`.
- **Frontend:** `Angular`, `HTML`, `CSS`.
- **Database:** `PostgreSQL`

<br>

## Deployment

The services used for deployment process are:

- **Backend:** `AWS Elastic Beanstalk`
- **Frontend:** `AWS S3`
- **Database:** `AWS RDS`

The services communicate with each other as in the following diagram:

![image](images/Architecture%20Diagram.jpg)

<br>

## Screenshots

- **AWS Elastic Beanstalk:**

![image](images/EB_01.png)

<br>

- **AWS S3:**

![image](images/S3_01.png)
![image](images/S3_02.png)
![image](images/S3_03.png)

<br>

- **AWS RDS:**

![image](images/RDS_01.png)
![image](images/RDS_02.png)

<br>

- **CircleCi:**

![image](images/CircleCi_01.png)
![image](images/CircleCi_02.png)
![image](images/CircleCi_03.png)