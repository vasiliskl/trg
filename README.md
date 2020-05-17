# TRG
The producer - consumer project

## User story
Data coming out of a sensor grid should be stored and processed for analytics and alerting purposes.
This data includes the location of each sensor in the grid (longitude, latitude) and also the sensor's measurements (humidity, temperature, pressure).

## Implementation
This should be implemented by 2 components, the producer and the consumer application.

The producer will provide a RESTful API that all the sensors in the network can call to submit their data.
This data will be added in a queue to be asynchronously processed and stored by the consumer components.

The code of the producer microservice can be found in the following link.

https://github.com/vasiliskl/trg-producer

The consumer application will consume the sensor data added by the producer, validate, store and process.

The code of the consumer microservice can be found in the following link.

https://github.com/vasiliskl/trg-consumer

More information about running the components and their tests, live metrics, Dockerfiles and how to scale is provided in each project.

## Technology
In this project, Quarkus framework with Apache Kafka and PostgreSQL were used.

https://quarkus.io/

https://www.cloudkarafka.com/

https://www.elephantsql.com/
