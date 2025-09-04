@Library('jenkins-shared-libraries')

def configMap = [
    component: "shipping",
    project: "roboshop"
]

if( ! env.BRANCH_NAME.configMap('main') ) {
    mavenEKSPipeline(configMap)
}
else{
    echo "Proceed to production"
}