pipeline {
  stages {


    stage('Docker build') {
        steps{
            sh 'docker build -t jenkins-leravel .'

        }
    }

    stage(' Run test') {
        steps {
            sh 'docker run jenkins-leravel php artisan ./vendor/bin/phpunit tests'
        }
    }
  }
}