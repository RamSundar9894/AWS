For installing Docker-Compose:
sudo curl -L "https://github.com/docker/compose/releases/download/v2.24.7/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
For TestNG:
wget https://repo1.maven.org/maven2/junit/junit/4.13.2/junit-4.13.2.jar
wget https://repo1.maven.org/maven2/org/hamcrest/hamcrest-core/1.3/hamcrest-core-1.3.jar
javac -cp .:junit-4.13.2.jar:hamcrest-core-1.3.jar src/Calculator.java test/CalculatorTest.java
java -cp .:src:test:junit-4.13.2.jar:hamcrest-core-1.3.jar org.junit.runner.JUnitCore CalculatorTest
