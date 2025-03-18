pipeline{
    agent any
    tools{
        jdk "JDK17"
        maven "MAVEN3.9"
    }
    environment {
        SNAP_REPO = 'vprofile-snapshort'
        NEXUS_USER = 'admin'
        NEXUS_PASS = 'admin123'
        RELEASE_REPO = 'vprofile-release'
        CENTAL_REPO = 'vpro-maven-central'
        NEXUSIP = '172.31.20.192'
        NEXUSPORT = '8081'
        NEXUS_GRP_REPO = 'vpro-maven-group'
        NEXUS_LOGIN = 'nexuslogin'



    }

    stages{
        stage('Build') {

            steps {
            
                sh 'mvn -s settings.xml -DskioTests install'
            }

        }



        


    }



}