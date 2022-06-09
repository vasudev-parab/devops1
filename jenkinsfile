pipeline {
    agent any

    stages
    {
        stage('build') 
        {
            steps 
            {
                echo 'Build App'
            }
        }
        stage('Test1') 
        {
            steps 
            {
                echo 'Test App'
            }
        }
        stage('Deploy') 
        {
            steps 
            {
                echo 'Deploy App'
            }
        }
    }
    
    post
    {
        
       always
        {
            emailext body: 'summary', subject: 'pipeline status', to: 'parab.vasu1992@gmail.com'
        }
    }
}
    
