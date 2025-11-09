# Postman API Automation with Github Actions  #

This repository is a demonstration for POC for integrating postman tests with Github actions. The tests are written in Postman and they are executed on the VM with the help of newman and newman-reporter-htmlextra. Github actions will trigger the project execution on every 
push to the main branch. You can also execute the project manually using workflow_dispatch. the projects run on a scheduled time with the help of cron job.

The HTML report is archived and kept in the artifact session for the team to download it. Along with that they can view the report directly from the github page : https://thineshkarthikeyan.github.io/Phoenix-Inwarranty-Flow/.
The latest report is mailed to the team members using GMAIL SMTP.

## About me ##
Hi, My name is Thinesh Kumaar. I have 6+ years of experience in Automation testing. My Skillsets includes UI Automation with Selenium Webdriver and cypress and for API testing Karate and Rest Assured. You can connect with me
over: (linkedin.com/in/thinesh-kumaar-536210282)



## Tech Stack ##
1. Postman
2. Nodejs 22
3. Newman
4. Newman-reporter-htmlextra
5. Github Actions
6. Gmail SMTP
7. Github Pages
8. AWS EC2 instance for self hosted github runner.

## Github Pages ##
You can directly view the latest test report of the Postman test at the Github page link : https://thineshkarthikeyan.github.io/Phoenix-Inwarranty-Flow/

## Testing Coverage ##
1. Happy Flow testing
2. Negative testing and edge case testing
3. Token testing
4. Schema validation
5. Secrets management with Github secrets

## HTML Report ##
The report will be created in the newman folder
![Postman Report](https://github.com/ThineshKarthikeyan/Phoenix-Inwarranty-Flow/blob/static-content/newman.JPG)

## Project Structure ##
```
Phoenix Inwarranty flow
├─ Inwarranty-flow Collection Copy.postman_collection.json      # Collection file
├─ QA.postman_environment.json                                  # Environment file
└─ testdata.csv

```

## How to run the Project ##
1. Clone the project on Local System: https://github.com/ThineshKarthikeyan/Phoenix-Inwarranty-Flow.git
2. Install Nodejs and NPM from https://nodejs.org/en/download
3. Install Newman and NPM from https://www.npmjs.com/
4. Install Newman using ``` npm install -g newman ```
5. Install Newman-reporter-htmlextra ``` npm install -g newman-reporter-htmlextra ```
6. Run the newman command:
7. ```    newman run 'Inwarranty-flow Collection Copy.postman_collection.json' \
          -e QA.postman_environment.json \
          -r cli,htmlextra \
          --reporter-htmlextra-export ./newman/index.html
   ```


       
