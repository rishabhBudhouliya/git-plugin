pipeline {
    agent none
    tools {
            maven 'maven-latest'
        }
    stages {
        stage('BuildAndTest') {
            matrix {
                agent any
                axes {
                		axis {
                	     		name 'os'
                	     		values 'CentOS-8', 'Debian-10', 'FreeBSD-12', 'windows'
                	     	  }
                	 }
                stages {
                    stage('Build') {
                        steps {
                            sh ''
                        }
                    }
                }
            }
        }
    }
}
