# testdata
testdata
mvn -U clean
mvn -DskipITs=true -Dmaven.test.skip=true package
mvn -Dmaven.test.skip=true -Dskip.integration.tests=true -Dskip.unit.tests=true --batch-mode -Dusername='${GITUSER}' -Dpassword='${PASSWD}' deploy


- curl -v --user admin:admin123 --upload-file <filename> http://localhost:8081/repository/<repository-name>/<filename>
