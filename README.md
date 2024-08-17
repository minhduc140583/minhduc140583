# Hi there

I am Duc Nguyen, a passionate open source contributor.
- 📫 Visit me at my [Linked In - Duc Nguyen](https://www.linkedin.com/in/duc-nguyen-437240239)


![A typical micro service](https://cdn-images-1.medium.com/max/800/1*d9kyekAbQYBxH-C6w38XZQ.png)

## 💼 Work
With my co-contributors, I created [core-go](https://github.com/core-go) and [core-ts](https://github.com/core-ts), which cover these areas:

### Database
- Simplify common database operations, such as CRUD (Create, Read, Update, Delete) operations, batch processing and transactions (for [SQL](https://github.com/core-go/sql)), by providing high-level abstractions and utilities.
- Generic CRUD Repository
    - It is like [CrudRepository](https://docs.spring.io/spring-data/commons/docs/current/api/org/springframework/data/repository/CrudRepository.html) of Spring, which promotes rapid development and consistency across applications.
    - While it provides many advantages, such as reducing boilerplate code and ensuring transactional integrity, it also offers flexibility and control over complex queries.
- My batis for GOLANG, nodejs
  - Project sample is at [go-admin](https://github.com/project-samples/go-admin). Mybatis file is here [query.xml](https://github.com/project-samples/go-admin/blob/main/configs/query.xml)
- Support:
    - [SQL](https://github.com/core-go/sql). The sample is at [go-sql-generic-sample](https://github.com/source-code-template/go-sql-generic-sample).
    - [Mongo](https://github.com/core-go/mongo). The sample is at [go-mongo-generic-sample](https://github.com/source-code-template/go-mongo-generic-sample).
    - [Cassandra](https://github.com/core-go/cassandra). The sample is at [go-cassandra-sample](https://github.com/source-code-template/go-cassandra-sample).
    - [Firestore](https://github.com/core-go/firestore). The sample is at [go-firestore-sample](https://github.com/go-tutorials/go-firestore-sample).
    - [Elastic Search](https://github.com/core-go/elasticsearch). The sample is at [go-elastic-search-generic-sample](https://github.com/source-code-template/go-elastic-search-generic-sample).
    - [Hive](https://github.com/core-go/hive). The sample is at [go-hive-sample](https://github.com/go-tutorials/go-hive-sample).
    - [Dynamodb](https://github.com/core-go/dynamodb). The sample is at [go-dynamodb-tutorial](https://github.com/go-tutorials/go-dynamodb-tutorial).

### Data Processing
Visit [core-go/io](https://github.com/core-go/io), you can see rich data processing:
- Import data from CSV or fix-length format files to [SQL](https://github.com/core-go/sql), [Mongo](https://github.com/core-go/mongo), [Cassandra](https://github.com/core-go/cassandra), [Firestore](https://github.com/core-go/firestore), [Elastic Search](https://github.com/core-go/elasticsearch), [Hive](https://github.com/core-go/hive)
- Export data from [SQL](https://github.com/project-samples/go-sql-export), [Mongo](https://github.com/project-samples/go-mongo-export), [Cassandra](https://github.com/project-samples/go-cassandra-export), [Firestore](https://github.com/project-samples/go-firestore-export), [Hive](https://github.com/project-samples/go-hive-export) to CSV or fix-length format files

### Message Queue
Please visit [core-go/mq](https://github.com/core-go/mq), Linked In article [Standardize-7-Message-Queues](https://www.linkedin.com/pulse/standardize-message-queues-golang-duc-nguyen-ekabc)
- Because message queues are a crucial component in modern software architecture, we support most of message queues, such as [Kafka](https://github.com/project-samples/go-kafka-sample), [RabbitMQ](https://github.com/project-samples/go-rabbit-mq-sample), [IBMMQ](https://github.com/project-samples/go-ibm-mq-sample), [Active MQ](https://github.com/project-samples/go-active-mq-sample), [NATS](https://github.com/project-samples/go-nats-sample), [Google Pub/Sub](https://github.com/project-samples/go-pubsub-sample), [Amazon SQS](https://github.com/project-samples/go-amazon-sqs-sample).
- Support 2 levels of 7 message queues:
    - Standardize and simplify 7 message queues, for 9 libraries [rabbitmq/amqp091-go](https://github.com/rabbitmq/amqp091-go), [aws-sdk-go/service/sqs](https://github.com/aws/aws-sdk-go/tree/main/service/sqs), [go/pubsub](https://pkg.go.dev/cloud.google.com/go/pubsub), [ibmmq](https://github.com/ibm-messaging/mq-golang), [ActiveMQ](https://github.com/go-stomp/stomp), [nats.go](https://github.com/nats-io/nats.go), [segmentio/kafka-go](https://github.com/segmentio/kafka-go), [IBM/sarama](https://github.com/IBM/sarama) and [Confluent](https://github.com/confluentinc/confluent-kafka-go).
    - Support standard level, which share the same interface with all message queues
        - Abstract the consumer flow
        - Support dead letter queue
    - Support SDK or original library level, you can use all advance features of the SDK/libraries

### Health Check
Please visit [core-go/health](https://github.com/core-go/health) and [Microservice Health Check](https://www.linkedin.com/pulse/microservice-health-check-go-nodejs-duc-nguyen-qunvc). We support databases, message queues, redis, http client:
- [http client](https://github.com/core-go/health/blob/main/http/health_checker.go)
- Redis: [go-redis/redis](https://github.com/core-go/health/blob/main/redis/v9/health_checker.go) to support [redis/go-redis](https://github.com/redis/go-redis), [garyburd/redigo](https://github.com/core-go/health/blob/main/redigo/health_checker.go) to support [gomodule/redigo](https://github.com/gomodule/redigo).
- Database: [sql](https://github.com/core-go/health/blob/main/sql/health_checker.go), [mongo](https://github.com/core-go/health/blob/main/mongo/health_checker.go), [dynamodb](https://github.com/core-go/health/blob/main/dynamodb/health_checker.go), [firestore](https://github.com/core-go/health/blob/main/firestore/health_checker.go), [elasticsearch](https://github.com/core-go/health/blob/main/elasticsearch/v8/health_checker.go), [cassandra](https://github.com/core-go/health/blob/main/cassandra/health_checker.go), [hive](https://github.com/core-go/health/blob/main/hive/health_checker.go)
- Message queues: [Kafka](https://github.com/project-samples/go-kafka-sample), [RabbitMQ](https://github.com/project-samples/go-rabbit-mq-sample), [IBMMQ](https://github.com/project-samples/go-ibm-mq-sample), [Active MQ](https://github.com/project-samples/go-active-mq-sample), [NATS](https://github.com/project-samples/go-nats-sample), [Google Pub/Sub](https://github.com/project-samples/go-pubsub-sample), [Amazon SQS](https://github.com/project-samples/go-amazon-sqs-sample).

![health](https://cdn-images-1.medium.com/max/800/1*NreJfea6tHobxMpiq96PPQ.png)

### Logging
Visit [core-go/log](https://github.com/core-go/log) and [Middleware-Log-Tracing](https://www.linkedin.com/pulse/middleware-log-tracing-go-duc-nguyen-uh0pc) for more details.
#### Providers
Standardize API for logging, support 2 libraries:
- [logrus](https://github.com/sirupsen/logrus)
- [zap](go.uber.org/zap)

#### Middleware Log Tracing
- [middleware](https://github.com/core-go/middleware): Log request and response at http middleware, allow to configure dynamic field names

#### Http Client Log Tracing
- [client](https://github.com/core-go/client): Log request and response at http client, allow to configure dynamic field names

#### Audit Log
- Support for CRUD, search (not required in every application). Sample is at [go-backoffice](https://github.com/project-samples/go-backoffice).

### Caching
#### Memory Cache
Refer to [MemoryCacheService](https://github.com/core-go/redis/blob/main/cache/memory_cache_service.go) for more details
- Time To Live: automatically clean up the expired objects in the memory cache
- Maximum size: When the memory exceeds the max size (which is configurable), it automatically remove the oldest object.
#### Redis
The library is here [Redis](https://github.com/core-go/redis). Support 2 libraries:
- [go-redis](https://github.com/go-redis/redis)
- [redigo](https://github.com/garyburd/redigo)

### Validator
Check required, email, url, min, max, country code, phone number, regular expression...
- [validator](https://github.com/core-go/validator)

### Search
Samples are [go-admin](https://github.com/project-samples/go-admin), [go-backoffice](https://github.com/project-samples/go-backoffice) and [go-location](https://github.com/project-samples/go-location)
- Generate the model by URL
- Paging
- Sort
#### Build a dynamic query for these providers
- SQL
- Mongo
- Dynamodb
- Firestore
- Elasticsearch

### Email
- Build some standard interfaces, which can be shared by multiple providers: SMTP and Sendgrid
- [mail](https://github.com/core-go/mail)
  - [smtp](https://github.com/core-go/mail/tree/main/smtp)
  - [sendgrid](https://github.com/core-go/mail/tree/main/sendgrid)
- The sample is [go-authentication](https://github.com/project-samples/go-authentication)

### Storage
- [storage](https://github.com/core-go/storage)
  - [Google](https://github.com/core-go/storage/tree/main/google)
  - [Amazon S3](https://github.com/core-go/storage/tree/main/s3)
- Samples are at [go-storage](https://github.com/project-samples/go-storage)

### Authentication 
Please visit [Authentication](https://github.com/core-go/authentication), we support:
- Support to log in by user name/password
- Login by LDAP (both server side and client slide)
- Login by Google, Facebook, Linkedin, Microsoft, Amazon, Dropbox
- Support any database design (SQL, Mongo, Firestore, Cassandra)

### Authorization
Please visit [security](https://github.com/core-go/security):
Sample is [go-admin](https://github.com/project-samples/go-admin)
- Identity and Access Management: Authorization at middleware, support http ([mux](https://github.com/gorilla/mux), [chi](https://github.com/go-chi/chi)), [gin](https://github.com/gin-gonic/gin), [echo](https://github.com/labstack/echo)
  - Support any database design (SQL, Mongo, Firestore, Cassandra)
- Crypto
- JWT

### Others
- [config](https://github.com/core-go/config)

## Summary:
- Libraries of core-go

![Collection of libraries of core-go](https://cdn-images-1.medium.com/max/800/1*bnsHDzTXilvfmI-HbNnK9Q.png)

### Cross-cutting concerns
![cross-cutting concerns](https://cdn-images-1.medium.com/max/800/1*y088T4NoJNrL9sqrKeSyqw.png)

### Hexagonal Architecture
![Hexagonal Architecture](https://cdn-images-1.medium.com/max/800/1*Dmf57O2Fkbx6kteaq5RVUw.png)

