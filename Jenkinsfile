def alert(alertMessage) {
    println("###########")
    println("# " + alertMessage)
    println("###########")
}


pipeline {
    agent any
    // parameters {
    //     string(name: 'ver', defaultValue: '0.1', description: 'pipeline version')
    // }

    stages {
        stage('get from scm') {
            steps {
                echo 'Hello World'
                //echo "Value from params: ${params.ver}"
                alert("this is message from groovy func 'alert'")
            }
        }
        
        stage('ver important step 2') {
            steps {
                echo 'Hello World'
                echo "Value from params: ${params.ver}"
                echo "env variable NAME: ${NAME}"
            }
        }
    }
}
