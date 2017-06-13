node {
        stage ('checkout') {
        checkout scm
    }

    stage ('debug') {
        bat 'powershell -command gci env: | ft -Auto'
        bat 'powershell -command gci -Recurse'
    
        if (BRANCH_NAME == 'master') {

            stage ('package') {
                echo 'Let\'s package because we\'re in master'
            }       
            stage ('publish') {
                echo 'Let\'s publish because we\'re in master'
            }       
            
        }
    }
}