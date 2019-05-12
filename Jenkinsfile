node('master') {
    stage ( 'git checkout' ) {
       git 'https://github.com/vinodsamant/jenkin.git' 
    }
    
     stage ('maven') {
     def dockerImage = 'maven:slim'
      docker.image(dockerImage).inside("-v ${WORKSPACE}:/root ") {
      sh " 'mvn' -Dmaven.test.failure.ignore clean install "
      }
  } 
