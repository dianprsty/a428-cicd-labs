// pipeline {
//     agent {
//         docker {
//             image 'node:16-buster-slim' 
//             args '-p 3001:3001' 
//         }
//     }
//     stages {
//         stage('Build') { 
//             steps {
// 		        sh 'yarn install'
//             }
//         }
// 		stage('Test') {
//             steps {
//                 sh './jenkins/scripts/test.sh'
//             }
//         }
        

//     }
// }

node {
	stage (‘Build’) {
		sh 'yarn install'
	}
	stage (‘Test’) {
		sh './jenkins/scripts/test.sh'
	}
}
