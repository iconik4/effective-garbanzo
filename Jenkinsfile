pipeline {
     agent {
         node {
             label "server"
           workspace "/mnt/"
         }
     }
     stages 
     {
         stage ('Print Message') {
             steps {
                 echo 'Hello world'
             }
         }
         stage ('HTTP Installation') {
             steps {
                 sh 'yum install httpd -y'
             }
         }
         stage ('HTTP Service start') {
             steps {
                 sh 'service httpd start'
             }
         }
     }
}
