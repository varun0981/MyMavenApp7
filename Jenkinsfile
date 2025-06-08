pipeline{
	agent any
tools{
	maven 'Maven'
	}
}
Stages{
	Stage('Checkout'){
	Steps{
		git branch:'master',url:''
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
		sh'mvn run'
		}
	}
}
