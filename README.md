# jwt-auth-nodejs
Basic JSON Web Token Auth with nodejs 

### Install Dependency
`npm install`

### Run
`node server.js`

#### To generate token use following curl

curl --request POST \
  --url http://localhost:8000/login \
  --header 'Accept: */*' \
  --header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6ImFkbWluQHRpbm55LmNvbSIsImlhdCI6MTU1OTk3NjE1NiwiZXhwIjoxNTYwMDYyNTU2fQ.Ppo5f6jmx4vuuvg1_OjvnE1c5qoyGQ8BQE9QfnwkKNI' \
  --header 'Cache-Control: no-cache' \
  --header 'Connection: keep-alive' \
  --header 'Content-Type: application/json' \
  --header 'Host: localhost:8000' \
  --header 'Postman-Token: 54ccde5f-c205-4c13-bed2-7583f049fd52,5be11e07-4264-4314-8ad4-ba36f0e449b5' \
  --header 'User-Agent: PostmanRuntime/7.13.0' \
  --header 'accept-encoding: gzip, deflate' \
  --header 'cache-control: no-cache' \
  --header 'content-length: 53' \
  --data '{"password":"admin!!!", "username":"admin@tinny.com"}'
  
  
 ### To check generated token use following curl
 
curl --request GET \
  --url http://localhost:8000 \
  --header 'Accept: */*' \
  --header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6ImFkbWluQHRpbm55LmNvbSIsImlhdCI6MTU1OTk3NjE1NiwiZXhwIjoxNTYwMDYyNTU2fQ.Ppo5f6jmx4vuuvg1_OjvnE1c5qoyGQ8BQE9QfnwkKNI' \
  --header 'Cache-Control: no-cache' \
  --header 'Connection: keep-alive' \
  --header 'Content-Type: application/json' \
  --header 'Host: localhost:8000' \
  --header 'Postman-Token: 9443908f-7946-4cdd-9ac8-8dc43fa95494,3a7c5e58-582d-4c53-bb06-548eb5ee36e3' \
  --header 'User-Agent: PostmanRuntime/7.13.0' \
  --header 'accept-encoding: gzip, deflate' \
  --header 'cache-control: no-cache'
  
  
  
