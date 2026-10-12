# Sample Springbot Project with Docker Deployment
## compiling
mvn clean install

## SwaggerUI
http://localhost:10000/swagger-ui/index.html#/Users/getAllUsers

## creating userservice image
docker build --no-cache -t userservice .

## running userservice image
docker run --rm -p 10000:10000 -e PORT=10000 userservice