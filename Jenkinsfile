

stage('Hello') {
    node {
        echo 'Hello World'
    }
}

stage('build docker') {
    node { 
        echo 'Hello Ofer'
        def myEnv = docker.build 'postgres'
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
