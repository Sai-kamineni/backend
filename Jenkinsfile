@Library('jenkins-shared-library') _ // gets the global pipeline libraries in system configuration

def configmap = [
    project: "expense",
    component: "backend"
]

if( ! env.BRANCH_NAME.equalsIgnoreCase('main')){ // true, if branch is feature branch
    nodeJSEKSPipeline(configmap)
}
else{
    echo "Follow the process of PROD release"
}