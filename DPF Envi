pipeline{
    agent any
    environment{
        FOO = "pipeline"
    }
    stages {
        stage("local"){
            environment{
            BAR = "stage"
            }
            steps {
                echo "${FOO} and ${BAR}"
            }
        }
        stage("global"){
            steps{
             echo "FOO is ${FOO}"
            }
        }
    }
}