properties([
    parameters([
        string(name: 'TARGET_ENV', defaultValue: 'test', description: 'test environment')
    ])
])
node{
            stage("test"){
                sh """
                    echo "This is test stage"
                    ls -ltr
                """
            }
        }