pipeline {
  agent any
  tools {
    maven "Maven"
  }
    stages {
        stage("build") {
            steps {
                echo "build …"
                 //snDevOpsStep()
                sleep 5
            }
        }
        stage("test") {
            steps {
                echo "test …"
                 //snDevOpsStep()
                sleep 5
            }
        }
        stage("Deploy for development") {
            when {
                branch "development"
            }
            steps {
                 echo "dev branch deployment …"
                 //snDevOpsStep()
                sleep 5
            }
        }
        stage("Deploy for production") {
            when {
                branch "production"
            }
            steps {
                echo "prod branch deployment …"
                 //snDevOpsStep()
                sleep 5
            }
        }
    }

