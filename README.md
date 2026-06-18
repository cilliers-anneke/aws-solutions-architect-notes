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
• AWS AppSync
• Amazon EventBridge (Amazon CloudWatch Events)
• Amazon MQ
• Amazon Simple Notification Service (Amazon SNS)
• Amazon Simple Queue Service (Amazon SQS)
• AWS Step Functions
Version 1.0 SAA-C03 12 | PAGE
AWS Cost Management:
• AWS Budgets
• AWS Cost and Usage Report
• AWS Cost Explorer
• Savings Plans
Compute:
• AWS Batch
• Amazon EC2
• Amazon EC2 Auto Scaling
• AWS Elastic Beanstalk
• AWS Outposts
• AWS Serverless Application Repository
• VMware Cloud on AWS
• AWS Wavelength
Containers:
• Amazon Elastic Container Registry (Amazon ECR)
• Amazon Elastic Container Service (Amazon ECS)
• Amazon ECS Anywhere
• Amazon Elastic Kubernetes Service (Amazon EKS)
• Amazon EKS Anywhere
• Amazon EKS Distro
Database:
• Amazon Aurora
• Amazon Aurora Serverless
• Amazon DocumentDB (with MongoDB compatibility)
• Amazon DynamoDB
• Amazon ElastiCache
• Amazon Keyspaces (for Apache Cassandra)
• Amazon Neptune
• Amazon Quantum Ledger Database (Amazon QLDB)
• Amazon RDS
• Amazon Redshift
• Amazon Timestream
Developer Tools:
• AWS X-Ray
Front-End Web and Mobile:
• AWS Amplify
• Amazon API Gateway
• AWS Device Farm
• Amazon PinpointVersion 1.0 SAA-C03 13 | PAGE
Machine Learning:
• Amazon Comprehend
• Amazon Forecast
• Amazon Fraud Detector
• Amazon Kendra
• Amazon Lex
• Amazon Polly
• Amazon Rekognition
• Amazon SageMaker
• Amazon Textract
• Amazon Transcribe
• Amazon Translate
Management and Governance:
• AWS Auto Scaling
• AWS CloudFormation
• AWS CloudTrail
• Amazon CloudWatch
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
