node {

    // def gitRepo = 'git@github.com:mano-organization/microservice-repo-1.git'
    // def gitCredentialsId = 'b70fe5f4-8191-4f7c-9108-c3806c4050bf'
    //def upstreamBranch = 'master'
    //checkout scm
    
    try {

        stage('Prepare') {
            // Get code from the git repository
            sh('echo "----> Buildingg..."')
            // git branch: upstreamBranch, credentialsId: gitCredentialsId, url: gitRepo
        }

        stage('Build') {

            sh('echo "----> Building..."')
           
        }

    }
    catch (err) {

        currentBuild.result = "FAILURE"
        throw err
    }

    finally {

        stage('Cleanup') {
            sh('echo "All Done"')
        }
    }
}
