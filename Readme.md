mvn archetype:generate -DgroupId=com.manning.apisecurityinaction -DartifactId=natter-api -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false


curl -i -d '{"name": "test space", "owner": "demo"}' http://localhost:4567/spaces
curl -i -d "{\"name\": \"test'space\", \"owner\": \"demo\"}"  http://localhost:4567/spaces
curl -i -d "{\"name\": \"test\",\"owner\": \"'); DROP TABLE spaces; --\"}" http://localhost:4567/spaces
