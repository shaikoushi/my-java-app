pipeline{
  agent any 
  stages{
    stage('git check out'){
      when{
        branch'test branch'
      }
      steps{
        echo'git checkout done'
      }
    }
      stage('sonar qube'){
      when{
        branch'develop'
      }
      steps{
        echo'static scan done'
      }
    }
      stage('maven build'){
      when{
        branch'uat branch'
      }
      steps{
        echo'maven build done'
      }
    }
      stage('nexus'){
      when{
        branch'upload '
      }
      steps{
        echo'uploading to nexus done'
      }
    }
  }
}
