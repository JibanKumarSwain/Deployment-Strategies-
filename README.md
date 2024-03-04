# Deployment-Strategies for AWS EC2-

## we have 4 type of deployment strategies

1- Recreate Deployment 

Delete all current servers and deploy new servers is known as Re-createing Deployment.

2- Rollback Deployment

if we have 3 servers of(version v1) application and 3 servers of(version v2) application    

thay i'll be replace one by one and thay use version2 v2 application if thay faceing any isseu    

thay back to version v1 application is known as Rolling back update Deployment 
   
3- Blue-green Deployment

if we have 4 servers v1 and we need to deploy new version v2 we need to create a 4 new servers 

thay run both and than we rediract some traffice to v2 servers if everthik will be ok then all 

traffice will be rediract to V2 servers is known as Blue-green Deployment.

4- Canary Deployment   
   
in this case if have 4 servers in version v1 application new version v2 we create some %10 or 20 

of traffice i'll be rediract to v2 if everythinks is ok then thay will rediract all traffice is 

known as Canary Deployment
