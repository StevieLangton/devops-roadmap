# 1. DevOps

### 1.1. What is DevOps?

**DevOps** is a software development methodology that combines software development (**Dev**) with information technology operations (**Ops**) participating together in the entire service lifecycle, from design through the development process to production support.

![DevOps Concepts](./docs/images/devops_concepts.png)

### 1.2. The goals of DevOps

* Fast Development Methodologies
* Fast Quality Assurance Methodologies
* Fast Deployment Methodologies
* Faster time to market
* Iteration & Continuous Feedback (strong and continuous communication between stakeholders – the end users and customers, product owners, development, quality assurance, and production engineers)

### 1.3. The benefits of DevOps

* **Environment Stabilization**

  *Enforces consistency, increase up-time*
* **Shorter Development Cycle**

  *Manage requirements and code-repository*
* **Increased Release Velocity**

  *Continuous build, push-button deployments*
* **Reduced Defects**

  *Regiment processes, automated testing*
* **Process Metrics**

  *Track both time at each stage, and the errors and exceptions*

![DevOps Benefits](./docs/images/devops_benefits.png)

### 1.4. The steps of DevOps

* **Plan**: task management, schedules
* **Code**: code development and code review, source code management tools, code merging
* **Build**: continuous integration tools, version control tools, build status
* **Test**: continuous testing tools that provide feedback on business risks, determine performance
* **Package**: artifact repository, application pre-deployment staging
* **Release**: change management, release approvals, release automation
* **Operate**: infrastructure installation, infrastructure changes (scalability), infrastructure configuration and management, infrastructure as code tools, capacity planning, capacity & resource management, security check, service deployment, high availability (HA), data recovery, log/backup management, database management
* **Monitor**: service performance monitoring, log monitoring, end user experience, incident management

![DevOps Steps](./docs/images/devops_steps.png)

### 1.5. Agile DevOps Process

![DevOps Process](./docs/images/devops_agile.png)

# 2. DevOps Technologies

![DevOps Technologies](./docs/images/devops_technologies.png)

## Roadmap for a DevOps developer
* **Step 1**: Learn a language
    * Begin with HTML & CSS
    * Learn basics of the JavaScript 
    * Understand TypeScript

  ***Reference:***
  https://github.com/leonardomso/33-js-concepts

* **Step 2**: Learn about source code management (recommend using Git)

  ***Reference:***
  https://github.com/k88hudson/git-flight-rules

* **Step 3**: Practice what you have learnt

* **Step 4**: Learn Package Manager

* **Step 5**: Learn about Unit Testing

* **Step 6**: Learn about databases (RDBMS & NoSQL)

* **Step 7**: Learn frameworks

* **Step 8**: Learn how to implement caching
    * Redis
    * Memcached

* **Step 9**: Creating RESTful APIs

* **Step 10**: Learn about different Authentication/Authorization methods

* **Step 11**: Understand Message Brokers
    * NSQ
    * Kafka
    * RabbitMQ
    * ZeroMQ

* **Step 12**: Learn how to use Docker

* **Step 13**: Knowledge of Web Servers

* **Step 14**: Learn how to test service
    * Test API
    * Test Performance
    * Test Security
    * Test Automation

* **Step 15**: Learn different protocols
    * TCP/UDP
    * Web Socket
    * AMQP
    * MQTT
    * Protocol Buffers
    * gRPC

* **Step 16**: Learn Microservice, Event Driven, Lambda architectures

* **Step 17**: Learn Big Data technologies/tools

* **Step 18**: Learn algorithms

  ***Reference:***
  https://github.com/TheAlgorithms/Python

* **Step 19**: Learn AI technologies

* **Step 20**: Learn configuration/deployment services

* **Step 21**: Learn how to monitor services

* **Step 22**: Use open source tools
  * Mock REST APIs: 
  https://github.com/typicode/json-server 

  * UML Designer:
  https://www.modelio.org

  * Planning: 
  https://wiki.gnome.org/Apps/Planner

  * MindMap: MindMaple Lite

  * UI Wireframe: Pencil (https://pencil.evolus.vn), Balsamiq

  * SSH clients for Windows: SuperPuTTY

* **Step 23**: Keep exploring

## 3. Big Data
### 3.1. What is Big Data?
A collection of **LARGE Datasets**, so it can **NOT be Processed** by traditional methods…

![Big Data Concept](./docs/images/bigdata_concept.png)

**[Source]**: https://topics.amcham.com.tw/wp-content/uploads/2016/03/BigData_2267x1146_white.png

### 3.2. Characteristics of Big Data
![Big Data Characteristics](./docs/images/bigdata_characteristics.png)

### 3.3. Big Data Use Cases
* Recommendation System
* Clickstream Analysis
* Real-time Analytics
* Sentiment Analysis
* Clustering Analysis
* Search
* Customer Segmentation
* Fraud Detection/Prevention
* Internet of Things
* Image Classification
* Anomaly Detection

### 3.4. Big Data Solutions
* <H3>Distributed File System</H3>

![Distributed File System](./docs/images/distributed_file_system.png)

* <H3>Distributed Database</H3>

![Distributed Database](./docs/images/distributed_database.png)

* <H3>Distributed Computation</H3>

![Distributed Computation](./docs/images/distributed_computation.png)

### 3.5. How Does Big Data Analysis Work?
![Distributed Computation](./docs/images/bigdata_flow.png)

### 3.6. Why Messing?
* Data usually flows from one application to another. It is produced by one application and used by one or more other applications. 
* Generally, the application **generating** or **sending** data is referred to as a **producer**, and the one **receiving** data is called a **consumer**.
* A simple way to send data from one application to another is to connect them to each other directly. However, tight coupling between producers and consumers requires them to be run at the same time or to implement a complex buffering mechanism. Therefore, **direct connections between producers and consumers does not scale**.

![Message Broker](./docs/images/message_broker.png)

**[Source]**: Apache Kafka

A **flexible** and **scalable** solution is to use a **message broker** or **messaging system**. Instead of applications connecting directly to each other, they connect to a message broker or a messaging system. This architecture makes it easy to add producers or consumers to a data pipeline.

### 3.7. What is Batch/Stream Processing?
* Batch processing is processing  a large volume of data at once.

  **Example** *processing  all the transactions that have been performed by a major ecommerce firm in a week. This data can tune into millions of records for a day which can be stored as a file/records etc. This particular file will undergo processing at the end of the day for various analysis the company wants to do and naturally it will take large amount of time for this to be processed. That would be what Batch processing is. And what Hadoop does is it provides Map Reduce as a processing tool for these large files which can be years of data stored monthly of data etc.*

* Stream processing changes the approach for processing. What it does is it applies the business logic to every transaction that is being recorded for the above ecommerce portal. It applies business logic to every event that is being captured rather than store all the events and then process them, which turns out now that whatever analysis is being done reflects the real state of the data at this instance. So, it becomes real time. And therefore stream processing is also associated with Real time.

<H3>Batch Processing vs Streaming Processing</H3>

| | Batch Processing | Stream Processing |
|-|-|-|
| **Data Scope** | Queries or processing over all or most of the data in the dataset | Queries or processing over data within a rolling time window, or on just the most recent data record |
| **Data Size** | Large batches of data | Individual records or micro batches consisting of a few records |
| **Performance** | Latencies in minutes to hours | Requires latency in the order of seconds or milliseconds |
| **Analyses** | Complex analytics | Simple response functions, aggregates, and rolling metrics |

## 4. Machine Learning
### 4.1. What is Machine Learning?
* Machine learning is creating and using models that are learned from data.
* Machine learning referred to as predictive modeling or data mining.

    **Examples**:
     * Spam prediction
     * Fraudulent credit card transaction prediction
     * A product or advertisement recommendation engine

<H3>Data Science Fields</H3>

![Data Science Fields](./docs/images/data_science_fields.png)

### 4.2. Traditional Programming vs Machine Learning
![Traditional Programming vs Machine Learning](./docs/images/traditional_programming_vs_machine_learning.png)

### 4.3. Machine Learning: Process
![Machine Learning: Process](./docs/images/machine_learning_process.png)

* <H3>Model Feedback Loop</H3>

![Model Feedback Loop](./docs/images/model_feedback_loop.png)

* <H3>Deep Learning Model Build/Deployment</H3>

![Model Feedback Loop](./docs/images/tensorflow_serving.png)

# 5. Books Recommendation
* **Best Seller in Computer Neural Networks on Amazon 2018**: *Hands-On Machine Learning with Scikit-Learn and TensorFlow* https://github.com/raycad/devops-roadmap/blob/master/books/ai/ml/hands_on_machine_learning_with_scikit_learn_and_tensorflow.pdf

* **System Design Primer**: https://github.com/raycad/devops-roadmap/blob/master/books/software-architecture/system_design_primer.pdf

* **Programming Collective Intelligence**: https://github.com/raycad/devops-roadmap/blob/master/books/ai/ml/oreilly_programming_collective_intelligence_aug_2007.pdf

* **Azure Cloud Architecture**: https://github.com/raycad/devops-roadmap/blob/master/books/software-architecture/azure_cloud_architecture.pdf

# 6. References

https://codeburst.io/the-2018-web-developer-roadmap-826b1b806e8d