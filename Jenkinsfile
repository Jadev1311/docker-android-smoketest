pipeline {
    agent { dockerfile true }
    stages {
        stage('Test') {
            steps {
                sh 'adb devices | grep emulator | cut -f 1'
            }
        }
    }
}