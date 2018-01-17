node {

    checkout scm

    appName = "hello-kenzan"
    imageName = "${appName}"
    env.BUILDIMG=imageName

    stage "Build"
    
        sh "docker build -t ${imageName} -f applications/hello-kenzan"
    
    /*stage "Push"

        sh "docker push ${imageName}"

    stage "Deploy"

        sh "sed 's#__IMAGE__#'$BUILDIMG'#' part1/hello-kenzan/k8s/deployment.yaml | kubectl apply -f -" */
}
