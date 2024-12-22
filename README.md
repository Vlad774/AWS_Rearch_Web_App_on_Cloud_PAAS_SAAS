# Lift and Shift Application Workload to AWS

## Description

This project refactors the vProfile web application by transitioning from traditional infrastructure to AWS PaaS and SaaS services for improved scalability, flexibility, and reduced operational overhead. It replaces EC2 instances with Elastic Beanstalk, RDS for MySQL, ElastiCache, and Amazon MQ to simplify management and improve performance. The use of Route 53 and CloudFront ensures efficient DNS management and content delivery globally.

## Technologies

- **Backend:** Spring MVC, Spring Security, Spring Data JPA.
- **Build/Deploy:** Maven, Tomcat.
- **Frontend:** JSP.
- **Database:** MySQL (via Amazon RDS).
- **Cache/Messaging:** Memcached (via ElastiCache), RabbitMQ (via Amazon MQ).
- **Search:** ElasticSearch.
- **DNS & CDN:** Route 53, CloudFront.

## Key AWS Services

- **Compute:** Elastic Beanstalk, EC2 (auto scaling), Application Load Balancer.
- **Storage:** Amazon S3 for artifact storage.
- **Database:** Amazon RDS for MySQL.
- **Cache/Messaging:** Amazon ElastiCache, Amazon MQ.
- **DNS & Security:** Amazon Route 53, Amazon CloudFront.
- **Monitoring & Automation:** CloudWatch for scaling and monitoring.

## Architecture Overview

- Elastic Beanstalk manages frontend EC2 instances, auto scaling, and load balancing.
- Backend services are handled by AWS managed services (RDS, ElastiCache, Amazon MQ).
- Requests are routed through Route 53 to CloudFront, which caches content globally.
- CloudWatch monitors resources and triggers scaling actions as needed.
  

## Walk-through:


 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/Diagramm.png) 
 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/artifact.png) 
 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/instances.png)
 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/volumes.png)
 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/security%20sgoup.png)
 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/target%20groups.png)
 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/autoscalling.png)
 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/backend.sh.png)


