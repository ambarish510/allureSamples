After cloning the repo, use following commands from the repo directory :-

git clone git@github.com:ambsFlip/allureSamples.git --branch mvn_testng_sample

cd maven-junit-jacoco-sample
mvn clean test
allure generate target/surefire-reports/
