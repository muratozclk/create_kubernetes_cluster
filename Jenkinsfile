pipeline {

    agent any
    stages {

            stage('Create Kubernetes Cluster') {
                steps {
                    sh "scp nodewebapp.yaml root@server-1:/tmp"
                    sh "ssh root@server-1 'kubectl apply -f /tmp/nodewebapp.yaml'"
                }
            }

        }
    }
