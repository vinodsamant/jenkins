node('master') {
    stage ( 'git checkout' ) {
       git 'https://github.com/vinodsamant/jenkin.git' 
    }
    
    stage('Compile-Package'){
        sh 'mvn package'
    }
 
}
