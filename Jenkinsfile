pipeline {
    agent { label 'mac' } // Specify the label for Mac OS agents

    stages {
        stage('Check Yarn Version') {
            steps {
                // Use brew to check the Yarn version on Mac OS
                sh 'brew install yarn && yarn --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                // Use brew to install Yarn and then install project dependencies
                sh 'brew install yarn && yarn install'
            }
        }
    }
}
