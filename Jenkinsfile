pipeline {
 agent any
 tools {
 maven "MAVEN3"
 jdk "OracleJDK8"
 }
 
 environment {
 SNAP_REPO = 'vprofile-snapshot'
 NEXUS_USER = 'admin'
 NEXUS_PASS = 'admin'
 RELEASE_REPO = 'vprofile-release'
 CENTRAL_REPO = 'maven-central-rey'
 NEXUSIP = '172.31.20.113'
 NEXUSPORT = '8081'
 NEXUS_GRP_REPO = 'vpro-maven-grp'
 NEXUS_LOGIN = 'nexuslogin'
 }
 stages {
 stage('Build'){
 steps {
 sh 'maven -s settings.xml -DskipTests install'
 }
 }
 }
}
