node('built-in')
 {
    stage('Continuous Download')
        {
        git branch: 'TESt', url: 'https://github.com/luniemma/Jnk2022.git'    
        }
    stage('Continuous Build')
         {
	input 'waiting for you to authorize'
	sh 'mvn package' 
        }
 }
