node('master') {
    stage ( 'SCM checkout' ) {
       git 'https://github.com/vinodsamant/jenkin.git' 
    }
    
    stage('Compile-Package'){
        sh 'mvn package'
    }
 
}
