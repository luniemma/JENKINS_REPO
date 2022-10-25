node('built-in')
 {
    stage('Continuous Download')
        {
        git branch: 'TESt', url: 'https://github.com/luniemma/Jnk2022.git'    
        }
    stage('Continuous Build')
         {
	echo 'building package'
	sh 'mvn package' 
        }
 }
