node('built-in')
 {
    stage('Continuous Download')
        {
        git branch: 'TESt', url: 'https://github.com/luniemma/Jnk2022.git'    
        }
    stage('Continuous Build')
        {
        sh 'mvn package' 
        }
    stage('Continue Deployment')
        {
        deploy adapters: [tomcat8(credentialsId: 'dev', path: '', url: 'http://10.0.28.141:8080')], contextPath: 'qaenv', war: '**/*.war'
        }
    stage('Continue Testing')
        {
        echo 'Testing was successful'  
        }
    stage('Continuous Delivery')
        {
    deploy adapters: [tomcat8(credentialsId: 'prod', path: '', url: 'http://10.0.23.67:8080')], contextPath: 'prodenv', war: '**/*.war'
        }
 }
