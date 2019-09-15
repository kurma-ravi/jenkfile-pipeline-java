node() {
    stage('Checkout') {
        checkout([$class: 'GitSCM', branches: [[name: 'master']], 
        doGenerateSubmoduleConfigurations: false, 
        extensions: [], 
        submoduleCfg: [], 
        userRemoteConfigs: [[url: 'https://github.com/kurma-ravi/pipeline-java.git']]])
     }
     
     stage('Compile') {
        bat "javac hello.java"
     }
  
     stage('Package') {
        echo "Packaging my app"
     }
}
