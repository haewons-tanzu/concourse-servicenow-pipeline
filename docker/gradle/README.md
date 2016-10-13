```
docker build -t pivotalservices/gradle .

# Get image id from running docker images 
docker tag c0f6b85c3be5 pivotalservices/gradle:2.14
docker tag c0f6b85c3be5 pivotalservices/gradle:latest

docker push pivotalservices/gradle
```
