# Procedure for job2:
- Firstly create a job in Jenkins
- Go to Source Code management section in configure of job2 .Give the details of the github repository and give the branch name as master branch by default it is set to master branch.
- Then go to trigger section select the option by which you want to trigger. In my case I used GITScm polling which checks the github repository evey minute and when there is a change in the github repository the job gets triggered depending on the schedule set
- Then go to build section where you need to write what you want to do while building. In my case I used shell scripting where the files downloaded from the github are put in a directory and this directory is mounted to the httpd docker image server
- Finally I could see the output required i.e. the Client side environment for deploying
