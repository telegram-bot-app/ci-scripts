# Telegram Bot App CI scripts

## General

The github actions workflows are shared across all the microservices and libraries within telegram-bot.app organisation.

## Workflow types

```build-test-publish.yaml` is used for the purpose of building microservices. It covers whole lifecycle of the microservice
  code from the commit to the release. It includes code static analysis, testing, scanning to finalize release with tagged docker image
  ready for deployment.

```library-test-publish.yaml` is used by the libraries within the project to aid with their release cycle. It does everything what the 
  build-test-publish does execept of building the docker image.
