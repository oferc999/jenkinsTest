

stage('Hello') {
    node {
        echo 'Hello World'
    }
}

stage('Ofer') {
    node { 
        echo 'Hello Ofer'
        def myEnv = docker.build 'my-environment:snapshot'
    }
}

stage('shell script') {
    node {
        sh 'ls -l'
        sh 'sleep 5'
        sh 'pwd'
    }
}
