pipeline { 
    agent any
    stages {
        stage('Clone Git') {
            steps {
                git 'https://github.com/bunkorner/Jenkins.git'
            }
        }
        stage('Build Code') {
            steps {
                chmod u+x Prog1.py
                ./Prog1.py
            }
        }
     stage('Test Code') {
            steps {
                chmod u+x Test.py
                ./Test.py
            }
        }
    } 
}
