# Information about API:
## Important
I have attached the references for the link with images but you have to download an then check the readme file
### Theme:
- We’re going to design an API for the doctors of a Hospital which has been allocated by the
govt for testing and quarantine + well being of COVID-19 patients
- There can be 2 types of Users
- Doctors
- Patients
- Doctors can log in
- Each time a patient visits, the doctor will follow 2 steps
- Register the patient in the app (using phone number, if the patient already exists, just
return the patient info in the API)
- After the checkup, create a Report
- Patient Report will have the following fields
- Created by doctor
- Status (You can use enums if you want to):
- Can be either of: [Negative, Travelled-Quarantine, Symptoms-Quarantine,
Positive-Admit]

- Date

# Instructions about SetUp:

First start with downloading the code and and write npm install on code editor, it will install all dependencies on your editor.
You will need a code editor and mongoDB setup on your computer.
We will use postman to check the api is working or not,So download postman on your computer.

1.Now use this **http://localhost:5000/api/v1/doctors/register** route to register doctor in API and add the info as shown in image

![image](./images/register%20doctor.png)

2.Use this **http://localhost:5000/api/v1/doctors/login** to login as a doctor and add info as shown in image

![image](./images/doctor%20login.png)

3.Use this **http://localhost:5000/api/v1/patients/register** and add the token in authorization area which is recieved in second point

![image](./images/register%20patient.png)

4. Use this **http://localhost:5000/api/v1/patients/62c31cc86a84003324d04cb5/create_report** to create report and add status you can see the types of 
   status in report model.

![image](./images/create%20report.png)

5.Use this **http://localhost:5000/api/v1/patients/register** to register patient

![image](./images/register%20patient.png)

6. Use this **http://localhost:5000/api/v1/patients/62c31cc86a84003324d04cb5/all_reports** to get all the reports.

![image](./images/all%20reports.png)


