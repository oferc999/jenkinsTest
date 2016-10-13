

stage('Hello') {
    node {
        echo 'Hello World'
    }
}

stage('build docker') {
    node { 
        echo 'Hello Ofer'
        // This step should not normally be used in your script. Consult the inline help for details.
        withDockerContainer(args: '--cap-add=SYS_ADMIN –P -d', image: 'checkpoint/centos-jenkins-agent') {
            // some block
        }
        
        
       // def postgres = docker.image('postgres:latest')
        //postgres.pull() // make sure we have the latest available from Docker Hub
        //postgres.inside {
            // …as above
        //}
        echo 'goinf to sleep 5 minutes'
        sh 'sleep 60'
    }
}

stage('shell script') {
    node {
        sh 'ls -l'
        sh 'sleep 5'
        sh 'pwd'
    }
}
