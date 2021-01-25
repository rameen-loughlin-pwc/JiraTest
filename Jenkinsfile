

stage('Deploy - Development') {
   when {
       branch 'master'
   }
   steps {
       echo 'Deploying to Production from master...'
   }
   post {
       always {
           jiraSendDeploymentInfo site: 'teachfirst.atlassian.net', environmentId: '', environmentName: '', environmentType: 'development'
       }
   }
}