pipeline {
       agent {
           label{
               label 'built-in'
                }
             }

       stages {

// Docker container stop and remove

            stage ('docker-container-stop') {
                steps{
                    sh "docker stop server1"
                    sh "docker stop server2"
                    sh "docker stop server3"
                    sh "docker stop server4"
                     }
                                            }

            stage ('docker container remove') {
                steps{
                    sh "docker system prune -a -f"
                     }
                                              }


             }

}
