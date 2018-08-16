node{
	stage('Check out'){
		git 'https://github.com/revceg/springbootwebapp-master'
	}
	stage('Test'){
		bat 'mvn test';
		junit 'target/surefire-reports/**/*.xml'
	} 
	stage('Build'){
		bat 'mvn clean package -DskipTests=true';
	}
  }
