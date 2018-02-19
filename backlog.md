## backlog project DeathStar 

    - [backlog project DeathStar](#backlog-project-deathstar)
        - [1 Base Cluster Design](#1-base-cluster-design)
            - [1.1 Infra-as-Code Deployment](#11-infra-as-code-deployment)
                - [1.1.1 Amazon Webservices](#111-amazon-webservices)
                    - [1.1.1.1 VPC](#1111-vpc)
                    - [1.1.1.2 Network Security Design](#1112-network-security-design)
                    - [1.1.1.3 Ingress Design](#1113-ingress-design)
                - [1.1.1.4 Persistant storage](#1114-persistant-storage)
                - [1.1.2 Microsoft Azure](#112-microsoft-azure)
                    - [1.1.2.1 Network Design](#1121-network-design)
                    - [1.1.2.2 Ingress Design](#1122-ingress-design)
            - [1.2 Authentication/Authorisation model](#12-authenticationauthorisation-model)
            - [1.3 Service Discovery](#13-service-discovery)
            - [1.4 DNS resolving](#14-dns-resolving)
        - [2 Services](#2-services)
            - [2.1 Metrics](#21-metrics)
            - [2.2 Log aggregation](#22-log-aggregation)
            - [2.3 Alerting](#23-alerting)
            - [2.4 Conformity scanning](#24-conformity-scanning)
            - [2.5 Application Deployment](#25-application-deployment)
            - [2.6 CI/CD integration](#26-cicd-integration)
            - [2.7 Code repository](#27-code-repository)
            - [2.8 Container Repository](#28-container-repository)

### 1 Base Cluster Design

Hoeveel clusters hebben we nodig en met welk doel ? 


#### 1.1 Infra-as-Code Deployment 

uitrol van een Kubernetes cluster vanuit een git repository, middels scripting

##### 1.1.1 Amazon Webservices

    Uitrol op Amazon web services.

###### 1.1.1.1 VPC

    Ontwerpen en implementeren van een netwerkdesign waarbij er rekening wordt gehouden met availebility zones en private en public subnets

###### 1.1.1.2 Network Security Design

    Ontwerp van een afdoende gesloten security group en network acl.

###### 1.1.1.3 Ingress Design

    Ontwerpen hoe netwerk verkeer het cluster binnen komt. 
    - Nginx ingress ?
    - Traefik ??

##### 1.1.1.4 Persistant storage

    Ontwerpen hoe we om gaan met persistente storage. 
    - waar komt deze storage vandaan? 
    - Welke backup policies zetten we in. 

##### 1.1.2 Microsoft Azure
    
    Uitrol op Microsoft Azure 

###### 1.1.2.1 Network Design

    Ontwerp implementatie van het netwerk design voor Azure installaties van een kubernetes cluster. 

###### 1.1.2.2 Ingress Design

    Ontwerpen hoe netwerk verkeer het cluster binnen komt. 
    - Nginx ingress ?
    - Traefik ?? 

#### 1.2 Authentication/Authorisation model

    Welke rollen, authorisaties en namespaces gaan we implementeren op het Cluster. 

    Wat wordt de authorisatie/authenticatie bron.

#### 1.3 Service Discovery

    Hoe gaan we service discovery inregelen

#### 1.4 DNS resolving

    Er moet een keuze gemaakt worden over het inregelen van DNS resloving richting het cluster. 

### 2 Services 

    Met services worden de diensten bedoeld die niet direct in het kubernetes cluster installatie plan zitten, maar die na uitrol van het cluster standaard meegeleverd worden om het cluster meteen productie klaar inzetbaar te maken. 

#### 2.1 Metrics

    Hoe gaan we metrics verzamelen. 
    Welke metrics gaan we verzamelen. 
    Wat zijn de parameters ten aanzien van Metrics collection? 

#### 2.2 Log aggregation
    
    Hoe gaan we logs weg zetten. 
    welke logs gaan we wegzetten. 

#### 2.3 Alerting
    
    Hoe gaan we alerts detecteren. 
    Waar gaan we de alerts heen sturen. 

#### 2.4 Conformity scanning

    Aan welke regels moeten draaiende containers voldoen en hoe/wie gaat dit handhaven. 

#### 2.5 Application Deployment

    Welke interfaces gaan we aanbieden richting het K8s cluster 

#### 2.6 CI/CD integration

    Op welke manier gaan we CI/CD faciliteren binnen het cluster. 

#### 2.7 Code repository

    Gaan we een centrale dienst aanbieden als code repository en waar komt deze dan te staan. 

#### 2.8 Container Repository

    Welke container repositories zijn toegestaan? 
    Gaan we er zelf een of meerdere aanbieden ? 
    

