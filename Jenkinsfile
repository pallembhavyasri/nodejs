properties([
    parameters([
        string(name: 'TARGET_ENV', defaultValue: 'test', description: 'test environment')
    ])
])
node{
    checkout scm
                stage("Install dependencies"){
                sh """
                    npm install
                """
            }
            stage("test"){
                sh """
                    echo "This is test stage"
                    ls -ltr
                """
            }
        }