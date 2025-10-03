properties([
    parameters([
        string(name: 'TARGET_ENV', defaultValue: 'test', description: 'test environment')
    ])
])
def appVersion = ''
node{
    checkout scm
            stage("Read the version"){
                script{
                def packageJson = readJSON file: 'package.json'
                appVersion = packageJson.version
                echo "app versions is $appVersion"

            }
            }
                stage("Install dependencies"){
                sh """
                    npm install
                    ls -ltr 
                    echo "app versions is $appVersion"
                """
            }
            stage("test"){
                sh """
                    echo "This is test stage"
                    ls -ltr
                """
            }
        }