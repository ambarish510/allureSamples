After cloning the repo, use following commands from the repo directory :-

git clone git@github.com:ambsFlip/allureSamples.git --branch mvn_testng_sample

cd allureSamples

mvn clean test

allure generate target/surefire-reports/
