# Spring
Real World Spring Projects

# Apache Kafka
<img width="626" height="319" alt="image" src="https://github.com/user-attachments/assets/e9072e4c-0764-46c4-9097-26369245aac5" />

- There can be multiple topics within Kafka. Each Topic can have multiple partitions furthur segregations.
<img width="972" height="526" alt="image" src="https://github.com/user-attachments/assets/205ac29b-c886-4919-ae27-2a5e6632b350" />

Offset -> Bookmark last message read.
<img width="982" height="521" alt="image" src="https://github.com/user-attachments/assets/3dadeae9-f313-4c10-8ffd-674d46b31977" />

Broker - One instance of Kafka.
<img width="973" height="513" alt="image" src="https://github.com/user-attachments/assets/9e9fbedc-274b-4e0c-9af9-c4d2df0cdbb3" />

<img width="955" height="399" alt="image" src="https://github.com/user-attachments/assets/57101431-4213-421b-85b9-45a0a6d24f83" />
<img width="974" height="296" alt="image" src="https://github.com/user-attachments/assets/fb6d2128-bb12-4033-beac-fa9f86d8c063" />

Terms:
<img width="831" height="456" alt="image" src="https://github.com/user-attachments/assets/6ccf8937-74f9-4f48-a385-4289835c229f" />

- String can easily be converted to byteArray but not Object. So, we need to make object serializable when publish to kafka topic.
  Why String works because Kafka provides: org.apache.kafka.common.serialization.StringSerializer

## Spring Cloud Stream
- Lets you write plain java functions and then "bind" them to messaging destinations (topics, queues) without writing any broker-specfic code.


# Kubernetes
- desigend to completely manage the lifecycle of containerized applications using methods that provide **predictability**, **scalability** and high **availability**.
- user can configure how applications should run and interact with outside world. Can run containers on any cloud or any region.

  ## Benefits
  - Service Discovery and Load Balancing
  - Automated Rollbacks and RollOuts to previous stable version
  - Horizontal Scaling (Scale out and scale down)
  - Self-Healing (Will automatically restart)
  - Secret and Configuration management ( deploy applicatino configurations without stopping containers and secure credentials using kubernetes secret)

  <img width="926" height="544" alt="image" src="https://github.com/user-attachments/assets/45587e73-3fe9-4f60-8e47-cc277cb1f3f1" />

  ## Minikube
   - Helps to run Kubernetes locally. It should not be used on production. On Production, AWS Kubernetes can be used to deploy on cloud.
   ### POD = Group of one or more containers and shared resources such as volumes(storage), IP Address and network ports. 
     - > Ephimeral = Can be created, scheduled and destroyed dynamically.
       > Pods not scale automatically
       > steteless = configurations need to be shared
       > Communicate with each-other localhost
       > Pos are assigned uniqe IP address within same cluster 

   ### Service
     - > single access point for pods and containers inside it.
       > LoadBalancer = Type of service to expose application to the outside world.
       > Replica Set = Idenetical Pods
          -> High Avalilability, Rolling Updates, Service Discovery and Load Balancing
          > Use selector to identify the pods it manages.

## Deployments

       




