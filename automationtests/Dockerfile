FROM openjdk:8

ENV maven_test_failure_ignore=${maven_test_failure_ignore}

ENV env_user=${env_user}

ENV env_endpoint=${env_endpoint}

ENV env_testLevel=${env_testLevel}

ENV userID=${userID}

ENV modules=${modules}

COPY ./target/automationtests-*-jar-with-dependencies.jar automationtests.jar

CMD ["java","-Dmaven.test.failure.ignore=${maven_test_failure_ignore}","-Denv.user=${env_user}","-Denv.endpoint=${env_endpoint}", "-Denv.testLevel=${env_testLevel}", "-DuserID=${userID}", "-Dmodules=${modules}","-jar","automationtests.jar"]
