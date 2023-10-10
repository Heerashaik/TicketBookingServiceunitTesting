pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
               //bat "rmdir  /s /q TicketBookingServiceunitTesting"
                bat "git clone https://github.com/Heerashaik/TicketBookingServiceunitTesting.git"
                bat "mvn clean -f TicketBookingServiceunitTesting"
            }
        }
        stage('install') {
            steps {
                bat "TicketBookingServiceunitTesting"
            }
        }
        stage('test') {
            steps {
                bat "TicketBookingServiceunitTesting"
            }
        }
        stage('package') {
            steps {
                bat "TicketBookingServiceunitTesting"
            }
        }
    }
}
