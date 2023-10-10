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
                bat "mvn install -f TicketBookingServiceunitTesting"
            }
        }
        stage('test') {
            steps {
                bat "mvn test -f TicketBookingServiceunitTesting"
            }
        }
        stage('package') {
            steps {
                bat "mvn package -f TicketBookingServiceunitTesting"
            }
        }
    }
}
