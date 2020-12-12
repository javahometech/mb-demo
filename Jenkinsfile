pipeline{
  agent any
  stages{
    stage("Maven Build"){
      steps{
        echo "building maven project"
      }
    }
    stage("Deploy To Dev"){
      when{
        branch 'dev'
      }
      steps{
        echo "deploying to dev"
      }
    }
  }
}
