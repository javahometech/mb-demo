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
    
    stage("Deploy To qa"){
      when{
        branch 'qa'
      }
      steps{
        echo "deploying to qa"
      }
    }
    
    stage("Deploy To prod"){
      when{
        branch 'main'
      }
      steps{
        echo "deploying to production"
      }
    }
  }
}
