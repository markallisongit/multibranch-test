node {
        stage ('checkout') {
        checkout scm
    }

    stage ('debug') {
        bat 'powershell -command gci env:'
    }
}