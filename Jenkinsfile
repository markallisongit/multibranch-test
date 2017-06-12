node {
        stage ('checkout') {
        checkout scm
    }

    stage ('debug') {
        bat 'powershell -command gci env:'
        bat 'powershell -command gci -Recurse'
    
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