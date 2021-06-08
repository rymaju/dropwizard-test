# Test Dropwizard

This is just a tiny hello world REST API built with Dropwizard to see how fast it is!

Using `loadtest`, and running it locally, I was able to get this basic API to yield ~1300 responses per seconds which is
a mean latency of about **0.8ms**.

That's super fast, no wonder why people like using Dropwizard...

How to start the test application
---

1. Run `mvn clean install` to build your application
1. Start application with `java -jar target/test-1.0-SNAPSHOT.jar server config.yml`
1. To check that your application is running enter url `http://localhost:8080`

Health Check
---

To see your applications health enter url `http://localhost:8081/healthcheck`
