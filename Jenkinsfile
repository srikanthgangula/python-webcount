pipeline {
    agent { label 'python3'}
    stages {
        stage ('clone the code') {
            steps {
                git url: 'https://github.com/srikanthgangula/python-webcount.gitt',
                    branch: 'master'
            }
        }

        stage ('install requirements') {
            steps {
                sh 'pip install -r requirements.txt'
                sh '/usr/share/man/man1/tox.1.gz/tox'
            }
        }
    }
}