pipeline {
    agent any
    tools { 
        maven 'Maven 3.3.9' 
    }
    stages {
        // stage('Checkout') {
        //     steps {
        //         checkout scm
        //     }
        // }

        stage('Build') {
            steps {
                sh 'mvn clean package' // или другая команда для сборки проекта
                bash 'pwd'
            }
        }

        // stage('Allure Report') {
        //     steps {
        //         sh 'mvn io.qameta.allure:allure-maven:serve'
        //     }
        // }

        // stage('Sonar Analysis') {
        //     steps {
        //         withSonarQubeEnv('SonarQube') {
        //             sh 'mvn sonar:sonar'
        //         }
        //     }
        // }

        // stage('Deployment') {
        //     steps {
        //         sh 'ansible-playbook deploy.yml' // или другая команда для деплоя через Ansible
        //     }
        // }
    }
}
