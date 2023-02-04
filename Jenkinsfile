/*stage("Git clone" {
    get credentialsID: 'GIT_HUB_CREDENTIAL', url: "https://github.com/shfy70/k8s.git"
}
*/

/*
podTemplate {
    node(POD_LABEL) {
        stage('Run shell') {
            sh 'echo fuck Biden'
        }
    }
}
*/

node {
  stage('Apply Kubernetes files') {
    withKubeConfig([credentialsId: 'user1', serverUrl: 'https://api.k8s.my-company.com']) {
      sh 'kubectl apply -f my-kubernetes-directory'
    }
  }
}

