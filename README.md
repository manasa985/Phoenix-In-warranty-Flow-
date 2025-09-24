# Postman API Automation Integration with Github actions #

This repositary is demonstrating  for POC for integrating postman test with github actions .
The rest are written in postman and are ececuted on VM with the help of new man and  newman -reporter-htmlextra.
Github Actions will trigger the project exection on every push to the main branch. you can also execute the project manually using workflow-aispatch . 
The project runs on a schedule time with the help of CRON job.

The HTML report is archived and kept in thr artifact secions for the team to download it. Along with they can view the report directly from the Github page:
The latest reports is mailed to the team members using Gmail SMTP.

##Tech stack##
1.Postman
2.NodeJs 22v
3.Newman
4.Newman Reporter htmlextra.
5.Github actions
6.Gmail SMTP
7.Githib pages
8.CSV for Data Driven Testing
9.AWS Ec2 instance for self hosted github runner.

## Github Pages##

## how to run the project##
 You can run the project on your local system for that 
 1. clone the project on local system. https://github.com/manasa985/Phoenix-In-warranty-Flow-.git
 2. Instal Nodejs and npm from https://nodejs.org/en/download
 3. install newman : $ npm install -g newman
 4. Install newman-reporter-htmlextra : npm install -g newman-reporter-htmlextra
 5. Run the newman cmd
     $ newman run 'Inwarranty-flow-Master-\ Collection.postman_collection.json'\
                               -e QA_Env_postman_environment.json \
                                -r cli,htmlextra \
                                --reporter-htmlextra-export. /newman/index.html

##Html Reprt##


