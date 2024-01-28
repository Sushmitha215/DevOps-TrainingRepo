pipeline{
    agent any
        stages{
            stage('checkout'){
                git checkout
            }
            stage('build'){
                // Maven or gradle(for Java) and .net cli for .Net and npm for angular and react
                mvn clean package

                //dotnet build

                //npm build
            }
            stage('test'){
                mvn test

               // dotnet test

               // npm test
            }
            stage('scan'){
                mvn sonar:sonar
            }

        }
}