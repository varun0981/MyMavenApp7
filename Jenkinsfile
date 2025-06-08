pipeline{
  agent any
  tools{
      maven 'Maven'
  }
stages{
	stage('Checkout'){
	Steps{
		git branch:'master',url:'https://github.com/varun0981/MyMavenApp7.git'
	}
}
	Stage('Build'){
	Steps{
		sh'mvn clean packages'
	}
}
	Stage('Test'){
	Steps{
		sh'mvn test'
	}
}
	Stage('Run Application'){
	Steps{
		sh'java -jar target/MyMavenApp7-1.0-SNAPSHOT.jar

	}
	}
}
}

