node{
    stage('validate'){
      sh  "terraform validate" 
    }
    stage('plan and create'){
    sh "echo creating gitRepos, teams, maven, sonarQube, nexus & k8s"
    sh "echo configurating maven, sonarQube, nexus & k8s"
    sh  "terraform plan" 
    sh  "terraform apply --auto-approve" 
    }
}