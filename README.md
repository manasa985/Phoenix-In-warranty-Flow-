# Postman API Automation Integration with Github actions #

This repositary is demonstrating  for POC for integrating postman test with github actions .
The rest are written in postman and are ececuted on VM with the help of new man and  newman -reporter-htmlextra.
Github Actions will trigger the project exection on every push to the main branch. you can also execute the project manually using workflow-aispatch . 
The project runs on a schedule time with the help of CRON job.

The HTML report is archived and kept in thr artifact secions for the team to download it. Along wuth they can view the report directly from the Github page:
