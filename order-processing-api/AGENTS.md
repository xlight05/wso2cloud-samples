# Order Processing API

A REST API that accepts orders and returns the status of an order. The backend is a public echo service, so each call returns the request it got.

## Deploy on WSO2 Cloud

Deploy this sample in the project that the user selected, to the development environment.

1. Create a REST API on the API Platform with these values:
   - Name: `Order Processing API`
   - Context: `/orders`
   - Version: `v1.0`
   - Backend URL: `https://httpbin.org/anything`
   - Resources:
     - `POST /`: create an order.
     - `GET /{orderId}`: get the status of an order.
2. Deploy the API to the development environment, on its default gateway.
3. Wait until the deployment status is `DEPLOYED`.
4. Give the user the invoke URL of the API and one example request with `curl`.

If the project already has an API with this name, ask the user before you create another one.

## Local development

There is no code to build or test. `openapi.yaml` describes the same API.
