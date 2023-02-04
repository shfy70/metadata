/*stage("Git clone" {
    get credentialsID: 'GIT_HUB_CREDENTIAL', url: "https://github.com/shfy70/k8s.git"
}
*/

podTemplate {
    node(POD_LABEL) {
        stage('Run shell') {
            sh 'kubectl get pods -n schweiz'
        }
    }
}