

stage('Hello') {
    node {
        echo 'Hello World'
    }
}

stage('build docker') {
    node { 
        echo 'Hello Ofer'
        def postgres = docker.image('postgres:latest')
        postgres.pull() // make sure we have the latest available from Docker Hub
        postgres.inside {
            // …as above
        }
        echo 'goinf to sleep 5 minutes'
        sh 'sleep 300'
    }
}

stage('shell script') {
    node {
        sh 'ls -l'
        sh 'sleep 5'
        sh 'pwd'
    }
}
