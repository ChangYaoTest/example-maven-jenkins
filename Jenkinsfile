pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
   after_success:
   - bash <(curl -s https://scripts.scantist.com/ci-jenkins.sh)
