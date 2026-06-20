# aws-solutions-architect-notes

My architectural design notes and hands-on lab configurations for the AWS SAA-C03 exam.

AWS services and features


Analytics:
• Amazon Athena  is an interactive query service that makes it easy to analyze data directly in
Amazon Simple Storage Service (Amazon S3) using standard SQL.

• AWS Data Exchange makes it easy to find, subscribe to, and use third-party data in the cloud. Qualified data providers include category-leading brands such as Reuters, who curate data from over 2.2 million unique news stories per year in multiple languages; Change Healthcare, who process and anonymize more than 14 billion healthcare transactions and $1 trillion in claims annually; Dun & Bradstreet, who maintain a database of more than 330 million global business records; and Foursquare, whose location data is derived from 220 million unique consumers and includes more than 60 million global commercial venues.

• AWS Data Pipeline is a web service that helps you reliably process and move data between different AWS compute and storage services, as well as on-premises data sources, at speciﬁed intervals. With AWS Data Pipeline, you can regularly access your data where it’s stored, transform and process it at scale, and eﬃciently transfer the results to AWS services such as Amazon S3, Amazon RDS, Amazon DynamoDB, and Amazon EMR.

• Amazon EMR is the industry-leading cloud big data platform for processing vast amounts of data using open source tools such as Apache Spark, Apache Hive, Apache HBase, Apache Flink, Apache Hudi, and Presto. Amazon EMR makes it easy to set up, operate, and scale your big data environments by automating time-consuming tasks such as provisioning capacity and tuning clusters. With Amazon EMR, you can run petabyte-scale analysis at less than half of the cost of traditional on-premises solutions and over 3x faster than standard Apache Spark. You can run workloads on Amazon EC2 instances, on Amazon Elastic Kubernetes Service (Amazon EKS) clusters, or on-premises using Amazon EMR on AWS Outposts.

• AWS Glue is a fully managed extract, transform, and load (ETL) service that makes it easy for customers to prepare and load their data for analytics. You can create and run an ETL job with a few clicks in the AWS Management Console. You simply point AWS Glue to your data stored in AWS, and AWS Glue discovers your data and stores the associated metadata (such as table definition and schema) in the AWS Glue Data Catalog. Once cataloged, your data is immediately searchable, queryable, and available for ETL.

• Amazon Kinesis makes it easy to collect, process, and analyze real-time, streaming data so you can get timely insights and react quickly to new information. Amazon Kinesis offers key capabilities to cost-effectively process streaming data at any scale, along with the flexibility to choose the tools that best suit the requirements of your application. With Amazon Kinesis, you can ingest real-time data such as video, audio, application logs, website clickstreams, and IoT telemetry data for machine learning (ML), analytics, and other applications. Amazon Kinesis enables you to process and analyze data as it arrives and respond instantly instead of having to wait until all your data is collected before the processing can begin.

• AWS Lake Formation is a service that makes it easy to set up a secure data lake in days. A data lake is a centralized, curated, and secured repository that stores all your data, both in its original form and prepared for analysis. A data lake enables you to break down data silos and combine different types of analytics to gain insights and guide better business decisions.

• Amazon Managed Streaming for Apache Kafka (Amazon MSK) is a fully managed service that makes it easy for you to build and run applications that use Apache Kafka to process streaming data. Apache Kafka is an open-source platform for building real-time streaming data pipelines and applications. With Amazon MSK, you can use Apache Kafka APIs to populate data lakes, stream changes to and from databases, and power ML and analytics applications. Apache Kafka clusters are challenging to setup, scale, and manage in production. When you run Apache Kafka on your own, you need to provision servers, configure Apache Kafka manually, replace servers when they fail, orchestrate server patches and upgrades, architect the cluster for high availability, ensure data is durably stored and secured, setup monitoring and alarms, and carefully plan scaling events to support load changes. Amazon MSK makes it easy for you to build and run production applications on Apache Kafka without needing Apache Kafka infrastructure management expertise. That means you spend less time managing infrastructure and more time building applications.
With a few clicks in the Amazon MSK console you can create highly available Apache Kafka clusters with settings and configuration based on Apache Kafka’s deployment best practices. Amazon MSK automatically provisions and runs your Apache Kafka clusters. Amazon MSK continuously monitors cluster health and automatically replaces unhealthy nodes with no downtime to your application. In addition, Amazon MSK secures your Apache Kafka cluster by encrypting data at rest.

• Amazon OpenSearch Service (Amazon Elasticsearch Service) makes it easy to deploy, secure, operate, and scale OpenSearch to search, analyze, and visualize data in real-time. With Amazon OpenSearch Service, you get easy-to-use APIs and real-time analytics capabilities to power use-cases such as log analytics, full-text search, application monitoring, and clickstream analytics, with enterprise-grade availability, scalability, and security. The service offers integrations with open-source tools such as OpenSearch Dashboards and Logstash for data ingestion and visualization. It also integrates seamlessly with other AWS services such as Amazon Virtual Private Cloud (Amazon VPC), AWS Key Management Service (AWS KMS), Amazon Data Firehose, AWS Lambda, AWS Identity and Access Management (IAM), Amazon Cognito, and Amazon CloudWatch, so that you can go from raw data to actionable insights quickly.

• Amazon OpenSearch Serverless is a serverless option in Amazon OpenSearch Service. As a developer, you can use OpenSearch Serverless to run petabyte-scale workloads without configuring, managing, and scaling OpenSearch clusters. You get the same interactive millisecond response times as OpenSearch Service with the simplicity of a serverless environment. The vector engine for Amazon OpenSearch Serverless, adds a simple, scalable, and high-performing vector storage and search capability to help developers build ML-augmented search experiences and generative AI applications without having to manage vector database infrastructure. Use cases for vector search collections include image search, document search, music retrieval, product recommendation, video search, location-based search, fraud detection, and anomaly detection.

• Amazon QuickSight (also known as Amazon Quick) is a cloud-based, serverless business intelligence (BI) service that enables you to build interactive dashboards, paginated reports, and embed analytics. It natively connects to data sources across AWS, allowing organizations to visualize insights and query data using AI.

• Amazon Redshift s the most widely used cloud data warehouse. It makes it fast, simple and cost-effective to analyze all your data using standard SQL and your existing Business Intelligence (BI) tools. It allows you to run complex analytic queries against terabytes to petabytes of structured and semi-structured data, using sophisticated query optimization, columnar storage on high-performance storage, and massively parallel query completion. Most results come back in seconds. You can start small for just $0.25 per hour with no commitments and scale out to petabytes of data for $1,000 per terabyte per year, less than a tenth the cost of traditional on-premises solutions.


Application Integration:

• Amazon AppFlow is a fully managed integration service that enables you to securely transfer data between Software-as-a-Service (SaaS) applications such as Salesforce, Zendesk, Slack, and ServiceNow, and AWS services such as Amazon S3 and Amazon Redshift, in just a few clicks. With Amazon AppFlow, you can run data flows at enterprise scale at the frequency you choose - on a schedule, in response to a business event, or on demand. You can configure data transformation capabilities such as filtering and validation to generate rich, ready-to-use data as part of the flow itself, without additional steps. Amazon AppFlow; automatically encrypts data in motion, and allows users to restrict data from flowing over the public internet for SaaS applications that are integrated with AWS PrivateLink, reducing exposure to security threats.

• AWS AppSync is a fully managed, serverless GraphQL and Pub/Sub API service. It simplifies application development by providing a single, secure endpoint to query, update, or publish real-time data across multiple data sources, such as Amazon DynamoDB and AWS Lambda.

• Amazon EventBridge (Amazon CloudWatch Events) is a serverless event bus that makes it easier to build event-driven applications at scale using events generated from your applications, integrated Software-as-a-Service (SaaS) applications, and AWS services. EventBridge delivers a stream of real-time data from event sources such as Zendesk or Shopify to targets such as AWS Lambda and other SaaS applications. You can set up routing rules to determine where to send your data to build application architectures that react in real-time to your data sources with event publisher and consumer completely decoupled.

• Amazon MQ  is a managed message broker service for Apache ActiveMQ Classic and RabbitMQ that makes it easy to set up and operate message brokers in the cloud. Message brokers allow different software systems–often using different programming languages, and on different platforms–to communicate and exchange information. Amazon MQ reduces your operational load by managing the provisioning, setup, and maintenance of ActiveMQ and RabbitMQ, popular open-source message brokers. Connecting your current applications to Amazon MQ is easy because it uses industry-standard APIs and protocols for messaging, including JMS, NMS, AMQP, STOMP, MQTT, and WebSocket. Using standards means that in most cases, there’s no need to rewrite any messaging code when you migrate to AWS.

• Amazon Simple Notification Service (Amazon SNS) is a highly available, durable, secure, fully managed pub/sub messaging service that enables you to decouple microservices, distributed systems, and serverless applications. Amazon SNS provides topics for high-throughput, push-based, many-to-many messaging. Using Amazon SNS topics, your publisher systems can fan out messages to a large number of subscriber endpoints for parallel processing, including Amazon SQS queues, AWS Lambda functions, and HTTP/S webhooks. Additionally, SNS can be used to fan out notifications to end users using mobile push, SMS, and email.

• Amazon Simple Queue Service (Amazon SQS) is a fully managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications. SQS eliminates the complexity and overhead associated with managing and operating message oriented middleware, and empowers developers to focus on differentiating work. Using Amazon SQS, you can send, store, and receive messages between software components at any volume, without losing messages or requiring other services to be available. Get started with Amazon SQS in minutes using the AWS Management Console, AWS CLI, or SDK of your choice, and three simple commands. Amazon SQS offers two types of message queues. Standard queues offer maximum throughput, best-effort ordering, and at-least-once delivery. Amazon SQS FIFO queues are designed to guarantee that messages are processed exactly once, in the exact order that they are sent.

• AWS Step Functions is a fully managed service that makes it easy to coordinate the components of distributed applications and microservices using visual workflows. Building applications from individual components that each perform a discrete function lets you scale easily and change applications quickly. Step Functions is a reliable way to coordinate components and step through the functions of your application. Step Functions provides a graphical console to arrange and visualize the components of your application as a series of steps. This makes it simple to build and run multi-step applications. Step Functions automatically initiates and tracks each step, and retries when there are errors, so your application runs in order and as expected. Step Functions logs the state of each step, so when things do go wrong, you can diagnose and debug problems quickly. You can change and add steps without even writing code, so you can easily evolve your application and innovate faster.


AWS Cost Management:

• AWS Budgets gives you the ability to set custom budgets that alert you when your costs or usage exceed (or are forecasted to exceed) your budgeted amount. You can also use AWS Budgets to set RI utilization or coverage targets and receive alerts when your utilization drops below the threshold you define. RI alerts support Amazon EC2, Amazon RDS, Amazon Redshift, and Amazon ElastiCache reservations. Budgets can be tracked at the monthly, quarterly, or yearly level, and you can customize the start and end dates. You can further refine your budget to track costs associated with multiple dimensions, such as AWS service, linked account, tag, and others. Budget alerts can be sent via email and/or Amazon Simple Notification Service (Amazon SNS) topic.Budgets can be created and tracked from the AWS Budgets dashboard or via the AWS Budgets API.

• AWS Cost and Usage Report is a single location for accessing comprehensive information about your AWS costs and usage. The AWS Cost and Usage Report lists AWS usage for each service category used by an account and its IAM users in hourly or daily line items, as well as any tags that you have activated for cost allocation purposes. You can also customize the AWS Cost and Usage Report to aggregate your usage data to the daily or monthly level.

• AWS Cost Explorer  has an easy-to-use interface that lets you visualize, understand, and manage your AWS costs and usage over time. Get started quickly by creating custom reports (including charts and tabular data) that analyze cost and usage data, both at a high level (such as total costs and usage across all accounts) and for highly-specific requests (such as m2.2xlarge costs within account Y that are tagged “project: secretProject”).

• Savings Plans is a flexible pricing model offering lower prices compared to On-Demand pricing, in exchange for a specific usage commitment (measured in $/hour) for a one or three-year period. AWS offers three types of Savings Plans – Compute Savings Plans, Amazon EC2 Instance Savings Plans, and Amazon SageMaker AI Savings Plans. Compute Savings Plans apply to usage across Amazon EC2, AWS Lambda, and AWS Fargate. The Amazon EC2 Instance Savings Plans apply to EC2 usage, and Amazon SageMaker AI Savings Plans apply to Amazon SageMaker AI usage. You can easily sign up a one- or three-year term Savings Plans in AWS Cost Explorer and manage your plans by taking advantage of recommendations, performance reporting, and budget alerts.


Compute:

• AWS Batch enables developers, scientists, and engineers to easily and efficiently run hundreds of thousands of batch computing jobs on AWS. AWS Batch dynamically provisions the optimal quantity and type of compute resources (such as CPU or memory-optimized instances) based on the volume and specific resource requirements of the batch jobs submitted. With AWS Batch, there is no need to install and manage batch computing software or server clusters that you use to run your jobs, allowing you to focus on analyzing results and solving problems. AWS Batch plans, schedules, and runs your batch computing workloads across the full range of AWS compute services and features, such as Amazon EC2 and Spot Instances.

• Amazon EC2 Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale computing easier for developers. The simple web interface of Amazon EC2 allows you to obtain and configure capacity with minimal friction. It provides you with complete control of your computing resources and lets you run on Amazon’s proven computing environment. Amazon EC2 reduces the time required to obtain and boot new server instances (called Amazon EC2 instances) to minutes, allowing you to quickly scale capacity, both up and down, as your computing requirements change. Amazon EC2 changes the economics of computing by allowing you to pay only for capacity that you actually use. Amazon EC2 provides developers and system administrators the tools to build failure resilient applications and isolate themselves from common failure scenarios.

• Amazon EC2 Auto Scaling helps you maintain application availability and allows you to automatically add or remove EC2 instances according to conditions you define. You can use the fleet management features of Amazon EC2 Auto Scaling to maintain the health and availability of your fleet. You can also use the dynamic and predictive scaling features of Amazon EC2 Auto Scaling to add or remove EC2 instances. Dynamic scaling responds to changing demand and predictive scaling automatically schedules the right number of EC2 instances based on predicted demand. Dynamic scaling and predictive scaling can be used together to scale faster.

• AWS Elastic Beanstalk is an easy-to-use service for deploying and scaling web applications and services developed with Java, .NET, PHP, Node.js, Python, Ruby, Go, and Docker on familiar servers such as Apache, Nginx, Passenger, and Internet Information Services (IIS). You can simply upload your code, and AWS Elastic Beanstalk automatically handles the deployment, from capacity provisioning, load balancing, and auto scaling to application health monitoring. At the same time, you retain full control over the AWS resources powering your application and can access the underlying resources at any time.

• AWS Outposts bring native AWS services, infrastructure, and operating models to virtually any data center, co-location space, or on-premises facility. You can use the same APIs, the same tools, the same hardware, and the same functionality across on-premises and the cloud to deliver a truly consistent hybrid experience. Outposts can be used to support workloads that need to remain on-premises due to low latency or local data processing needs. AWS Outposts come in two variants: 
VMware Cloud on AWS Outposts allows you to use the same VMware control plane and APIs you use to run your infrastructure. AWS-native variant of AWS Outposts allows you to use the same exact APIs and control plane you use to run in the AWS Cloud, but on-premises. AWS Outposts infrastructure is fully managed, maintained, and supported by AWS to deliver access to the latest AWS services. Getting started is easy, you simply log into the AWS Management Console to order your Outposts servers, choosing from a wide range of compute and storage options. You can order one or more servers, or quarter, half, and full rack units.

• AWS Serverless Application Repository The AWS Serverless Application Repository enables you to quickly deploy code samples, components, and complete applications for common use cases such as web and mobile backends, event and data processing, logging, monitoring, Internet of Things (IoT), and more. Each application is packaged with an AWS Serverless Application Model (AWS SAM) template that defines the AWS resources used. Publicly shared applications also include a link to the application’s source code. There is no additional charge to use the AWS Serverless Application Repository - you only pay for the AWS resources used in the applications you deploy. You can also use the AWS Serverless Application Repository to publish your own applications and share them within your team, across your organization, or with the community at large. To share an application you've built, publish it to the AWS Serverless Application Repository

• VMware Cloud on AWS is an integrated cloud offering jointly developed by AWS and VMware delivering a highly scalable, secure and innovative service that allows organizations to seamlessly migrate and extend their on-premises VMware vSphere-based environments to the AWS Cloud running on next-generation Amazon Elastic Compute Cloud (Amazon EC2) bare metal infrastructure. VMware Cloud on AWS is ideal for enterprise IT infrastructure and operations organizations looking to migrate their on-premises vSphere-based workloads to the public cloud, consolidate and extend their data center capacities, and optimize, simplify and modernize their disaster recovery solutions.

• AWS Wavelength is an AWS Infrastructure offering optimized for mobile edge computing applications. Wavelength Zones are AWS infrastructure deployments that embed AWS compute and storage services within communications service providers’ (CSP) datacenters at the edge of the 5G network, so application traffic from 5G devices can reach application servers running in Wavelength Zones without leaving the telecommunications network. This avoids the latency that would result from application traffic having to traverse multiple hops across the Internet to reach their destination, enabling customers to take full advantage of the latency and bandwidth benefits offered by modern 5G networks.


Containers:

• Amazon Elastic Container Registry (Amazon ECR) is a fully managed Docker container registry that makes it easy for developers to store, manage, and deploy Docker container images. Container images are managed, stored, and deployed through Amazon Elastic Container Registry (ECR), a fully managed container registry service. These images serve as the standalone, executable blueprints used to run containerized applications across various AWS compute services. Amazon ECR is integrated with Amazon Elastic Container Service (Amazon ECS), simplifying your development to production workﬂow. Amazon ECR eliminates the need to operate your own container repositories or worry about scaling the underlying infrastructure. Amazon ECR hosts your images in a highly available and scalable architecture, allowing you to reliably deploy containers for your applications. Integration with AWS Identity and Access Management (IAM) provides resource-level control of each repository. With Amazon ECR, there are no upfront fees or commitments. You pay only for the amount of data you store in your repositories and data transferred to the internet.

• Amazon Elastic Container Service (Amazon ECS) is a highly scalable, high-performance container orchestration service that supports Docker containers and allows you to easily run and scale containerized applications on AWS. Amazon ECS eliminates the need for you to install and operate your own container orchestration software, manage and scale a cluster of virtual machines (VMs), or schedule containers on those VMs. With simple API calls, you can launch and stop Docker-enabled applications, query the complete state of your application, and access many familiar features such as IAM roles, security groups, load balancers, Amazon CloudWatch Events, CloudFormation templates, and AWS CloudTrail logs.

• Amazon ECS Anywhere  Anywhere is a feature of Amazon ECS that lets you run and manage container workloads on your infrastructure. This feature helps you meet compliance requirements and scale your business without sacrificing your on-premises investments.

• Amazon Elastic Kubernetes Service (Amazon EKS) makes it easy to deploy, manage, and scale containerized applications using Kubernetes on AWS. Amazon EKS runs the Kubernetes management infrastructure for you across multiple AWS Availability Zones to eliminate a single point of failure. Amazon EKS is certified Kubernetes conformant so you can use existing tooling and plugins from partners and the Kubernetes community. Applications running on any standard Kubernetes environment are fully compatible and can be easily migrated to Amazon EKS.

• Amazon EKS Anywhere is a container management software that enables organizations to create, operate, and manage Kubernetes clusters on their own on-premises infrastructure or edge environments. Built on the same open-source distribution used by AWS, it allows you to maintain a consistent hybrid cloud experience without managing the underlying cloud resources.

• Amazon EKS Distro  is an open-source Kubernetes distribution built and maintained by AWS. It provides the exact same upstream Kubernetes binaries, configurations, and dependencies that power the managed Amazon EKS service in the cloud, allowing developers to run consistent, production-grade Kubernetes clusters anywhere.


Database:

• Amazon Aurora is a MySQL and PostgreSQL compatible relational database engine that combines the speed and availability of high-end commercial databases with the simplicity and cost-effectiveness of open source databases. Amazon Aurora is up to five times faster than standard MySQL databases and three times faster than standard PostgreSQL databases. It provides the security, availability, and reliability of commercial databases at 1/10th the cost. Amazon Aurora is fully managed by Amazon Relational Database Service (Amazon RDS), which automates time-consuming administration tasks such as hardware provisioning, database setup, patching, and backups. Amazon Aurora features a distributed, fault-tolerant, self-healing storage system that auto-scales up to 128TB per database instance. It delivers high performance and availability with up to 15 low-latency read replicas, point-in-time recovery, continuous backup to Amazon S3, and replication across three Availability Zones (AZs). Amazon Aurora I/O-Optimized is a cluster conﬁguration that oﬀers improved price performance and predictable pricing for customers with I/O-intensive applications, such as e-commerce applications, payment processing systems, and financial applications. Aurora-Optimized oﬀers improved performance, increasing throughput and reducing latency to support your most demanding workloads, with up to 40 percent cost savings when your I/O spend exceeds 25 percent of your current Aurora database spend. Amazon Aurora MySQL zero-ETL integration with Amazon Redshift, now available in public preview, enables near real-time analytics and machine learning of data stored in Aurora MySQL-Compatible Edition. Transactional data written to Aurora is available to you in Amazon Redshift within seconds, without building and maintaining complex data pipelines.

• Amazon Aurora Serverless is an on-demand, auto-scaling configuration for MySQL- and PostgreSQL-compatible databases. It automatically starts up, shuts down, and scales compute capacity up or down based on application demands, allowing you to pay only for the exact resources you consume. 

• Amazon DocumentDB (with MongoDB compatibility) is a fast, scalable, highly available, and fully managed document database service that supports MongoDB workloads. Amazon DocumentDB is designed from the ground-up to give you the performance, scalability, and availability you need when operating mission-critical MongoDB workloads at scale. Amazon DocumentDB implements the Apache 2.0 open source MongoDB 3.6 and 4.0 APIs by emulating the responses that a MongoDB client expects from a MongoDB server, allowing you to use your existing MongoDB drivers and tools with Amazon DocumentDB (with MongoDB compatibility).

• Amazon DynamoDB is a key-value and document database that delivers single-digit millisecond performance at any scale. It's a fully managed, multi-Region database with built-in security, backup and restore, and in-memory caching for internet-scale applications. DynamoDB can handle more than 10 trillion requests per day and support peaks of more than 20 million requests per second. Many of the world's fastest growing businesses such as Lyft, Airbnb, and Redfin, as well as enterprises such as Samsung, Toyota, and Capital One, depend on the scale and performance of DynamoDB to support their mission-critical workloads. Hundreds of thousands of AWS customers have chosen DynamoDB as their key-value and document database for mobile, web, gaming, ad tech, Internet of Things (IoT), and other applications that need low-latency data access at any scale. Create a new table for your application and let DynamoDB handle the rest.

• Amazon ElastiCache is a web service that makes it easy to deploy, operate, and scale an in-memory cache in the cloud. The service improves the performance of web applications by allowing you to retrieve information from fast, managed, in-memory caches, instead of relying entirely on slower disk-based databases. ElastiCache supports two open-source in-memory caching engines: Redis — a fast, open-source, in-memory key-value data store for use as a database, cache, message broker, and queue. Amazon ElastiCache (Redis OSS) is a Redis-compatible in-memory service that delivers the ease-of-use and power of Redis along with the availability, reliability, and performance suitable for the most demanding applications. Both single-node and up to 15-shard clusters are available, enabling scalability to up to 3.55 TiB of in-memory data. Amazon ElastiCache (Redis OSS) is fully managed, scalable, and secure. This makes it an ideal candidate to power high-performance use cases such as web, mobile apps, gaming, ad-tech, and IoT. Memcached — a widely adopted memory object caching system. Amazon ElastiCache (Memcached) is protocol compliant with Memcached, so popular tools that you use today with existing Memcached environments will work seamlessly with the service. 
Amazon ElastiCache Serverless is a serverless option for Amazon ElastiCache that simplifies cache management and instantly scales to support the most demanding applications. With ElastiCache Serverless, you can create a highly available and scalable cache in less than a minute, eliminating the need to plan for, provision, and manage cache cluster capacity. ElastiCache Serverless automatically stores data redundantly across multiple Availability Zones (AZs) and provides a 99.99% availability Service Level Agreement (SLA). With ElastiCache Serverless, you pay for data stored and compute consumed by your workload, with no upfront commitments or additional costs.

• Amazon Keyspaces (for Apache Cassandra) is a scalable, highly available, and managed Apache Cassandra–compatible database service. With Amazon Keyspaces, you can run your Cassandra workloads on AWS using the same Cassandra application code and developer tools that you use today. You don’t have to provision, patch, or manage servers, and you don’t have to install, maintain, or operate software. Amazon Keyspaces is serverless, so you pay for only the resources you use and the service can automatically scale tables up and down in response to application traffic. You can build applications that serve thousands of requests per second with virtually unlimited throughput and storage. Data is encrypted by default and Amazon Keyspaces enables you to back up your table data continuously using point-in-time recovery. Amazon Keyspaces gives you the performance, elasticity, and enterprise features you need to operate business-critical Cassandra workloads at scale.

• Amazon Neptune is a fast, reliable, fully managed graph database service that makes it easy to build and run applications that work with highly connected datasets. The core of Amazon Neptune is a purpose-built, high-performance graph database engine optimized for storing billions of relationships and querying the graph with milliseconds latency. Amazon Neptune supports popular graph models Property Graph and W3C's RDF, and their respective query languages Apache TinkerPop Gremlin and SPARQL, allowing you to easily build queries that efficiently navigate highly connected datasets. Neptune powers graph use cases such as recommendation engines, fraud detection, knowledge graphs, drug discovery, and network security. Amazon Neptune is highly available, with read replicas, point-in-time recovery, continuous backup to Amazon S3, and replication across Availability Zones. Neptune is secure with support for encryption at rest. Neptune is fully managed, so you no longer need to worry about database management tasks such as hardware provisioning, software patching, setup, configuration, or backups. 
Amazon Neptune Analytics is an analytics database engine for quickly analyzing large volumes of graph data to get insights and find trends from data stored in Amazon S3 buckets or a Neptune database. Neptune Analytics uses built-in algorithms, vector search, and in-memory computing to run queries on data with tens of billions of relationships in seconds.

• Amazon Quantum Ledger Database (Amazon QLDB) is a fully managed, serverless ledger database that provides a transparent, immutable, and cryptographically verifiable transaction log owned by a central trusted authority. It was culled in 2025.

• Amazon RDS makes it easy to set up, operate, and scale a relational database in the cloud. It provides cost-efficient and resizable capacity while automating time-consuming administration tasks such as hardware provisioning, database setup, patching and backups. It frees you to focus on your applications so you can give them the fast performance, high availability, security and compatibility they need. Amazon RDS is available on several database instance types—optimized for memory, performance or I/O—and provides you with six familiar database engines to choose from, including MySQL, MariaDB, PostgreSQL, Oracle Database, Microsoft SQL Server, and Amazon RDS on AWS Outposts. You can use the AWS Database Migration Service to easily migrate or replicate your existing databases to Amazon RDS.

• Amazon Redshift is a fully managed, petabyte-scale cloud data warehouse optimized for running complex business intelligence (BI) queries against massive, structured datasets using columnar storage.

• Amazon Timestream is a fast, scalable, fully managed time series database service for IoT and operational applications that makes it easy to store and analyze trillions of events per day at 1/10th the cost of relational databases. Driven by the rise of IoT devices, IT systems, and smart industrial machines, time series data — data that measures how things change over time — is one of the fastest growing data types. Time-series data has specific characteristics such as typically arriving in time order form, data is append-only, and queries are always over a time interval. While relational databases can store this data, they are inefficient at processing this data as they lack optimizations such as storing and retrieving data by time intervals. Timestream is a purpose-built time series database that efficiently stores and processes this data by time intervals. With Timestream, you can easily store and analyze log data for DevOps, sensor data for IoT applications, and industrial telemetry data for equipment maintenance. As your data grows over time, the Timestream adaptive query processing engine understands its location and format, making your data simpler and faster to analyze. Timestream also automates rollups, retention, tiering, and compression of data, so you can manage your data at the lowest possible cost. Timestream is serverless, so there are no servers to manage. It manages time-consuming tasks such as server provisioning, software patching, setup, configuration, or data retention and tiering, freeing you to focus on building your applications.


Developer Tools:

• AWS X-Ray helps developers analyze and debug distributed applications in production or under development, such as those built using a microservices architecture. X-Ray, you can understand how your application and its underlying services are performing so you can identify and troubleshoot the root cause of performance issues and errors. X-Ray provides an end-to-end view of requests as they travel through your application, and shows a map of your application’s underlying components. You can use X-Ray to analyze both applications in development and in production, from simple three-tier applications to complex microservices applications consisting of thousands of services. Under service since Feb 2026


Front-End Web and Mobile:

• AWS Amplify is a set of purpose-built tools and features that lets frontend web and mobile developers quickly build, deploy, and host full-stack applications on AWS without manually configuring the underlying infrastructure.. It makes it easy to create, configure, and implement scalable mobile applications powered by AWS. Amplify seamlessly provisions and manages your mobile backend and provides a simple framework to easily integrate your backend with your iOS, Android, Web, and React Native frontends. Amplify also automates the application release process of both your front-end and back-end allowing you to deliver features faster. Mobile applications require cloud services for actions that can’t be done directly on the device, such as offline data synchronization, storage, or data sharing across multiple users. You often have to configure, set up, and manage multiple services to power the backend. You also have to integrate each of those services into your application by writing multiple lines of code. However, as the number of application features grow, your code and release process becomes more complex and managing the backend requires more time. Amplify provisions and manages backends for your mobile applications. You just select the capabilities you need such as authentication, analytics, or offline data sync, and Amplify will automatically provision and manage the AWS service that powers each of the capabilities. You can then integrate those capabilities into your application through the Amplify libraries and UI components.

• Amazon API Gateway is one of the most critical structural components of Domain 2 (Resilient Architectures) and Domain 3 (High-Performing Architectures) on the SAA-C03 blueprint. It is the core service used to achieve loose coupling and build serverless microservices. is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure REST, HTTP, and WebSocket APIs at any scale, acting as a secure traffic cop for backend services.

• AWS Device Farm is an app testing service that lets you test and interact with your Android, iOS, and web apps on many devices at once, or reproduce issues on a device in real time. View video, screenshots, logs, and performance data to pinpoint and fix issues before shipping your app.

• Amazon PinpointVersion AWS has officially announced that Amazon Pinpoint will end support on October 30, 2026. AWS is actively migrating its features into two separate, modern destinations: Amazon Connect (for multi-channel campaigns and customer journeys) and AWS End User Messaging (for high-volume transactional SMS, push notifications, and emails).is a fully managed, outbound marketing communication and customer engagement service designed to segment audiences and deliver targeted multi-channel messages (SMS, email, push notifications, and voice).


Machine Learning:
• Amazon Comprehend uses ML and natural language processing (NLP) to help you uncover the insights and relationships in your unstructured data. The service identifies the language of the text; extracts key phrases, places, people, brands, or events; understands how positive or negative the text is; analyzes text using tokenization and parts of speech; and automatically organizes a collection of text files by topic. You can also use AutoML capabilities in Amazon Comprehend to build a custom set of entities or text classification models that are tailored uniquely to your organization’s needs. For extracting complex medical information from unstructured text, you can use Amazon Comprehend Medical. The service can identify medical information, such as medical conditions, medications, dosages, strengths, and frequencies from a variety of sources like doctor’s notes, clinical trial reports, and patient health records. Amazon Comprehend Medical also identifies the relationship among the extracted medication and test, treatment and procedure information for easier analysis. For example, the service identifies a particular dosage, strength, and frequency related to a specific medication from unstructured clinical notes. Amazon Comprehend is a fully managed, serverless Natural Language Processing (NLP) service that uses machine learning to look at unstructured text and instantly extract deep insights, entities, sentiment, and patterns without requiring any ML expertise.

• Amazon Forecast is a fully managed, serverless time-series forecasting service that uses machine learning to analyze historical sequence data and accurately predict future business trends with zero ML experience required.AWS officially closed access to new customers for Amazon Forecast back in July 2024. AWS now redirects all active development for these specific workloads to the low-code time-series engine inside Amazon SageMaker Canvas.  

• Amazon Fraud Detector is a fully managed, serverless AI service designed to automate the creation of customized machine learning models that detect online scams—like payment fraud and fake account creations—in milliseconds with zero ML experience.uses ML and natural language processing (NLP) to help you uncover the insights and relationships in your unstructured data. The service identifies the language of the text; extracts key phrases, places, people, brands, or events; understands how positive or negative the text is; analyzes text using tokenization and parts of speech; and automatically organizes a collection of text files by topic. You can also use AutoML capabilities in Amazon Comprehend to build a custom set of entities or text classification models that are tailored uniquely to your organization’s needs. For extracting complex medical information from unstructured text, you can use Amazon Comprehend Medical. The service can identify medical information, such as medical conditions, medications, dosages, strengths, and frequencies from a variety of sources like doctor’s notes, clinical trial reports, and patient health records. Amazon Comprehend Medical also identifies the relationship among the extracted medication and test, treatment and procedure information for easier analysis. For example, the service identifies a particular dosage, strength, and frequency related to a specific medication from unstructured clinical notes.

• Amazon Kendra is an intelligent search service powered by ML. Amazon Kendra reimagines enterprise search for your websites and applications so your employees and customers can easily find the content they are looking for, even when it’s scattered across multiple locations and content repositories within your organization.Using Amazon Kendra, you can stop searching through troves of unstructured data and discover the right answers to your questions, when you need them. Amazon Kendra is a fully managed service, so there are no servers to provision, and no ML models to build, train, or deploy.

• Amazon Lex  is a fully managed artificial intelligence (AI) service to design, build, test, and deploy conversational interfaces into any application using voice and text. Lex provides the advanced deep learning functionalities of automatic speech recognition (ASR) for converting speech to text, and natural language understanding (NLU) to recognize the intent of the text, to enable you to build applications with highly engaging user experiences and lifelike conversational interactions, and create new categories of products. With Amazon Lex, the same deep learning technologies that power Amazon Alexa are now available to any developer, enabling you to quickly and easily build sophisticated, natural language, conversational bots (“chatbots”) and voice enabled interactive voice response (IVR) systems. Amazon Lex enables developers to build conversational chatbots quickly. With Amazon Lex, no deep learning expertise is necessary—to create a bot, you just specify the basic conversation flow in the Amazon Lex console. Amazon Lex manages the dialogue and dynamically adjusts the responses in the conversation. Using the console, you can build, test, and publish your text or voice chatbot. You can then add the conversational interfaces to bots on mobile devices, web applications, and chat platforms (for example, Facebook Messenger). There are no upfront costs or minimum fees to use Amazon Lex - you are charged only for the text or speech requests that are made. The pay-as-you-go pricing and the low cost per request make the service a cost-effective way to build conversational interfaces. With the Amazon Lex free tier, you can easily try Amazon Lex without any initial investment.

• Amazon Polly is a service that turns text into lifelike speech. Amazon Polly lets you create applications that talk, enabling you to build entirely new categories of speech-enabled products. Amazon Polly is an Amazon artificial intelligence (AI) service that uses advanced deep learning technologies to synthesize speech that sounds like a human voice. Amazon Polly includes a wide selection of lifelike voices spread across dozens of languages, so you can select the ideal voice and build speech-enabled applications that work in many different countries. Amazon Polly delivers the consistently fast response times required to support real-time, interactive dialog. You can cache and save Amazon Polly speech audio to replay offline or redistribute. And Amazon Polly is easy to use. You simply send the text you want converted into speech to the Amazon Polly API, and Amazon Polly immediately returns the audio stream to your application so your application can play it directly or store it in a standard audio file format, such as MP3. In addition to Standard TTS voices, Amazon Polly offers Neural Text-to-Speech (NTTS) voices that deliver advanced improvements in speech quality through a new machine learning approach. Polly’s Neural TTS technology also supports a Newscaster speaking style that is tailored to news narration use cases. Finally, Amazon Polly Brand Voice can create a custom voice for your organization. This is a custom engagement where you will work with the Amazon Polly team to build an NTTS voice for the exclusive use of your organization.

• Amazon Rekognition makes it easy to add image and video analysis to your applications using proven, highly scalable, deep learning technology that requires no ML expertise to use. With Amazon Rekognition, you can identify objects, people, text, scenes, and activities in images and videos, as well as detect any inappropriate content. Amazon Rekognition also provides highly accurate facial analysis and facial search capabilities that you can use to detect, analyze, and compare faces for a wide variety of user verification, people counting, and public safety use cases. With Amazon Rekognition Custom Labels, you can identify the objects and scenes in images that are specific to your business needs. For example, you can build a model to classify specific machine parts on your assembly line or to detect unhealthy plants. Amazon Rekognition Custom Labels takes care of the heavy lifting of model development for you, so no ML experience is required. You simply need to supply images of objects or scenes you want to identify, and the service handles the rest.

• Amazon SageMaker you can build, train, and deploy ML models for any use case with fully managed infrastructure, tools, and workflows. SageMaker AI removes the heavy lifting from each step of the ML process to make it easier to develop high-quality models. SageMaker AI provides all of the components used for ML in a single toolset so models get to production faster with much less effort and at lower cost.

• Amazon Textract is a serverless machine learning service that goes beyond simple Optical Character Recognition (OCR) to automatically extract text, handwriting, tables, and structured form data from scanned documents and PDFs. 

• Amazon Transcribe is a fully managed, serverless speech-to-text service that uses advanced deep learning models to convert live audio streams or pre-recorded audio files into highly accurate, time-stamped text.

• Amazon Translate is a serverless, neural machine translation service that delivers fast, high-quality, and affordable language translation across dozens of global languages.


Management and Governance:

• AWS Auto Scaling monitors your applications and automatically adjusts capacity to maintain steady, predictable performance at the lowest possible cost.

• AWS CloudFormation is an Infrastructure as Code (IaC) service that allows you to model, provision, and manage a collection of related AWS resources predictably and repeatedly using JSON or YAML templates.

• AWS CloudTrail is a governance, compliance, and operational auditing service that records every single API call and action taken within your AWS account.

• Amazon CloudWatch is an Infrastructure as Code (IaC) service that allows you to model, provision, and manage a collection of related AWS resources predictably and repeatedly using JSON or YAML templates.

• AWS Command Line Interface (AWS CLI)

• AWS Compute Optimizer

• AWS Config

• AWS Control Tower

• AWS License Manager

• Amazon Managed Grafana

• Amazon Managed Service for Prometheus

• AWS Management Console

• AWS Organizations

• AWS Personal Health Dashboard

• AWS Proton

• AWS Service Catalog

• AWS Systems Manager

• AWS Trusted Advisor

• AWS Well-Architected Tool


Media Services:

• Amazon Elastic Transcoder

• Amazon Kinesis Video Streams


Migration and Transfer:

• AWS Application Discovery Service

• AWS Application Migration Service (CloudEndure Migration)

• AWS Database Migration Service (AWS DMS)

• AWS DataSync

• AWS Migration Hub

• AWS Server Migration Service (AWS SMS)

• AWS Snow Family

• AWS Transfer Family


Networking and Content Delivery:

• Amazon CloudFront

• AWS Direct Connect

• Elastic Load Balancing (ELB)

• AWS Global Accelerator

• AWS PrivateLink

• Amazon Route 53

• AWS Transit Gateway

• Amazon VPC

• AWS VPN


Security, Identity, and Compliance:

• AWS Artifact

• AWS Audit Manager

• AWS Certificate Manager (ACM)

• AWS CloudHSM

• Amazon Cognito

• Amazon Detective

• AWS Directory Service

• AWS Firewall Manager

• Amazon GuardDuty

• AWS Identity and Access Management (IAM)

• Amazon Inspector

• AWS Key Management Service (AWS KMS)

• Amazon Macie

• AWS Network Firewall

• AWS Resource Access Manager (AWS RAM)

• AWS Secrets Manager

• AWS Security Hub

• AWS Shield

• AWS Single Sign-On

• AWS WAF


Serverless:

• AWS AppSync

• AWS Fargate

• AWS Lambda


Storage:

• AWS Backup

• Amazon Elastic Block Store (Amazon EBS)

• Amazon Elastic File System (Amazon EFS)

• Amazon FSx (for all types)

• Amazon S3

• Amazon S3 Glacier

• AWS Storage Gateway

