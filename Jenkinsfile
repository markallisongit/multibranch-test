node {
        stage ('checkout') {
        checkout scm
    }

    stage ('debug') {
        bat 'powershell -command gci env:'
    }

    if (${BRANCH_NAME} == 'master') {
        echo 'Let\'s package because we\'re in master'
    }
}