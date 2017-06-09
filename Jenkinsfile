node {
        stage ('checkout') {
        checkout scm
    }

    stage ('debug') {
        bat 'powershell -command gci env:'
    
        if (BRANCH_NAME == 'master') {

            stage ('package') {
                echo 'Let\'s package because we\'re in master'
            }       
            stage ('publish') {
                echo 'Let\'s package because we\'re in master'
            }       
            
        }
    }
}