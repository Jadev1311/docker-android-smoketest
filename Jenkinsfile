pipeline {
    agent { dockerfile true }
    stages {
        stage('Test') {
            steps {
                sh 'adb devices | grep emulator | cut -f 1'
                sh 'appium -p 4723 -bp 2251 --default-capabilities '{"udid":"'${udid}'"}' &'
            }
        }
    }
}