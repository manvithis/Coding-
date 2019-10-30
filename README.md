# Coding-

#curl -4 icanhazip.com -to get ip-address from pinging from thirdparty website

#DOCKER:

docker info 

docker search $IMAGE

docker -i image /bin/bash

docker commit $CONTAINER_id $TO_IMAGE

docker diff $CONTAINER_id  (for the changes made in container)

docker images ps -a
docker container ps -a
docker stop $CONTAINER_id
docker rm $CONTAINER_id

Dockerfile:
docker run -t NAME .

FROM
RUN
COPY
CMD
ENTRYPOINT

os.environ[NAME]
docker run -e NAME=$$$$ for running the environment variables

*If the environment variable is defined both in Dockerfile and as a flag, then the command flag takes precedence.

to remove all the containers which are stopped
docker rm $(docker ps --no-trunc -aq)





# jenkins:

To make master node not run any jobs set executions jobs to 0 and let slave nodes handle them




      Pipeline{

         agent any{
   
            stages{

            #ANY CONDITIONS

              stage('Checkout'){
                git url: "URL"
              }
              stage('compile'){
              }
              stage('test'){
              }
              stage('deplot'){
              }
            }
          }
      }


Tools for codeTesting Automation or CodeQuality control:
JaCoCo, Clover, and Cobertura

##alternative to CQ:sonarQube  :Learn this thing by MID_NOV
 
     triggers {
      pollSCM('* * * * *')
      }
      
      
/etc
# ┌- minute (0 - 59)
# │ ┌- hour (0 - 23)
# │ │ ┌─day of the month (1 - 31)
# │ │ │ ┌──month (1 - 12)
# │ │ │ │ ┌────────day of the week (0 - 6) (Sunday to Saturday;
# │ │ │ │ │                                   7 is also Sunday on some systems)
# │ │ │ │ │
# │ │ │ │ │
# * * * * * command to execute



    post {
     always {
          mail to: 'team@company.com',
          subject: "Completed Pipeline: ${currentBuild.fullDisplayName}",
          body: "Your build completed, please check: ${env.BUILD_URL}"
            }
      }
always: Execute regardless of the completion status

changed: Execute only if the pipeline changed its status

failure: Execute only if the pipeline has the failed status

success: Execute only if the pipeline has the success status

unstable: Execute only if the pipeline has the unstable status (usually caused by test failures or code violations)





# kubernetes
