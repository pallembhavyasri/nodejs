properties([
    parameters([
        string(name: 'TARGET_ENV', defaultValue: 'tes', description: 'test environment')
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