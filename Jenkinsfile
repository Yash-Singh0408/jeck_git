pipeline{
  agent any

  stages{
    stage('fetch fil'){
      steps{
        git 'https://github.com/Yash-Singh0408/jeck_git.git'
      }
    }
    stage('Building'){
      steps{
        echo 'Building Project _________'
        bat 'javac test1.java
      }
    }
    stage('Executing'){
      steps{
        echo 'Executing ________'
        bat 'java test1'
      }
    }
    stage('Deploy'){
      steps{
        echo 'Deploying ________'
      }
    }
    post{
      success{
        echo "Pipeline executed successfully."
      }
      failure{
        echo "Pipeline failed."
    }
  }
}
