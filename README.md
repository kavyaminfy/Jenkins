# Jenkins

## Pipeline
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'sleep 5'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'sleep 3'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                sh 'sleep 2'
            }
        }
    }
    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline execution failed!'
        }
    }
}


## Jenkins Dashboard (showing job list and executor).
![image](https://github.com/user-attachments/assets/ee1d0c91-5186-4ee9-b673-c228384a346a)


## Stage View of successful pipeline

![image](https://github.com/user-attachments/assets/67d4af54-fae4-4474-a4a3-ae16f81cb410)

![image](https://github.com/user-attachments/assets/1f30a39d-2188-4edc-b2f2-42694298add4)
## After Configure 
![image](https://github.com/user-attachments/assets/c39872be-320a-47a6-a97e-3647949e9819)



## Console Output
![image](https://github.com/user-attachments/assets/c43d1585-c6cb-482c-ac46-703587be43d2)
## After Configure 
![image](https://github.com/user-attachments/assets/633f4a1d-e544-4cbf-8082-6b27b1f3cce7)


While working on this Jenkins pipeline, I got a good hang of how to set up and run a basic pipeline job using the Jenkins interface. I checked out the dashboard, build queue, and stage view to see how things flow. Watching each stage run and checking the logs gave me a clear idea of what’s happening behind the scenes. Adding a new stage was simple and showed me how flexible pipelines are. Overall, it was a good hands-on way to get comfortable with Jenkins and how it handles automation.
