# Deployment-Strategies for AWS EC2-

## we have 4 type of deployment strategies     

----------------------------------------------------------------------
--------------------------------------------------------------------
     
# Deployment Strategies: What Are They     

To successfully launch a new version of the software solution they provide, DevOps teams use deployment strategies. Using these techniques, 
network traffic in a production environment is transitioned from the old version to the new version based on the firm's specialty. 
Deployment strategies can influence downtime and operational costs based on the company's specialty.

## Deployment Strategies of Different Types     

Now that we know what deployment strategies are, let's explore the different types of deployment strategies.
    
## Deployment in blue and green

This deployment strategy involves running the new version of the software alongside the old version. Note that this is also known as a red/black deployment strategy.

Stable or older versions of the application are always blue or red, while newer versions are green or black.

When the new version has been tested and certified to meet all the requirements, the load balancer automatically switches traffic from the older version to the newer one.

In addition to offering a quick update or rollout of a new application version, this strategy has the disadvantage of being
expensive since both the new and old versions must run simultaneously. Engineers mostly use this method in mobile app development and deployment.

## Canary Deployments

During canary deployment, the team responsible for deployment gradually redirects traffic from the older version to the new one. 
For instance, at a certain stage in the process, 90% of production traffic may still go through the older version while only 10% goes 
through the newer one. This approach allows DevOps engineers to evaluate the stability of the new version by using live traffic from 
a subset of end-users at varying levels throughout production.

Canary Deployments enables better performance monitoring as well as faster and easier software rollbacks. However, it has a slow deployment cycle and requires more time.

## Recreate Deployment

The development team shuts down the old version of the application completely, deploys the new version, then reboots the whole system. 
This deployment method produces a system downtime between shutting down the old software and booting the new one.

As there is no traffic shifting from one version to another in the live production environment, it requires no load balancer.

The downtime in this strategy, however, affects the end user dramatically. Users must wait until the application is live again to use it.
As a result, not many developers use this strategy unless it is their only option.
