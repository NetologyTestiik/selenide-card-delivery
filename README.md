# Card Delivery Automation Tests

![CI Pipeline](https://github.com/NetologyTestiik/selenide-card-delivery/actions/workflows/ci.yml/badge.svg)

Homework for Netology course "2.2. Selenide"

## Description
Automated tests for card delivery form submission using Selenide and JUnit 5.

## Technologies
- Java 11
- Selenide 6.19.1
- JUnit 5
- Gradle

## Run tests locally
```bash
# Start application
java -jar artifacts/app-card-delivery.jar

# In another terminal, run tests
./gradlew test
```

## Run tests in headless mode
```bash
./gradlew test -Dselenide.headless=true
```

## Project structure
- `artifacts/app-card-delivery.jar` - application under test
- `src/test/java/ru/netology/CardDeliveryTest.java` - test class
- `.github/workflows/ci.yml` - CI/CD pipeline
- `build.gradle` - build configuration

## Test scenarios
1. Successful form submission with valid data
2. Date generation: current date + 3 days
