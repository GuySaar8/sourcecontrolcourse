pipeline {
  agent any
  stages {
    stage('Create File') {
      steps {
        sh '''

echo "Guy Saar" > /home/guy/Desktop/my_name.txt
'''
      }
    }

    stage('Read File') {
      steps {
        sh 'cat /home/guy/Desktop/my_name.txt'
      }
    }

    stage('Check Disk Space') {
      steps {
        sh 'df -h /dev/sda1 /dev/sda'
      }
    }

    stage('Move File') {
      steps {
        sh '''mv /home/guy/Desktop/my_name.txt /home/guy/Desktop/new_folder/my_name.txt 
'''
      }
    }

  }
}