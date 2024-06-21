#!groovy
@library('roboshop-shared-library') _

// responsibility to pass what type of component is this to pipeline decision

def configMap = [
    application: "nodejsVM"
    component: "catalogue"
]

if( ! env.BRANCH_NAME.equalsIgnoreCase('main')){
    pipelineDecission.decidePipeline(configMap)
}
else{
    echo "This is PRODUCTION, deal with CR process"
}