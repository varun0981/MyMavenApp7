pipeline{
  agent any
  tools{
      maven 'Maven'
  }
stages{
	stage('Checkout'){
	steps{
		git branch:'master',url:'https://github.com/varun0981/MyMavenApp7.git'
	}
}
	stage('Build'){
	steps{
		sh'mvn clean package'
	}
}
	stage('Test'){
	steps{
		sh'mvn test'
	}
}
	stage('Run Application'){
	steps{
		sh'java -jar target/MyMavenApp7-1.0-SNAPSHOT.jar'

	}
	}
}
}

