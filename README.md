# CST8915 Lab 3 - Algonquin Pet Store

## Architecture
- RabbitMQ -> Azure Virtual Machine
- Product service -> Azure Web App
- Order service -> Azure Web App
- Store front -> Azure Virtual Machine

The Store front gets products from the Product service and sends orders to the Order service. The Order service sends orders to RabbitMQ.

## Service URLs
- [Product service](https://product-service-lab3-bout0167-dcc7fwgsajfbbubr.mexicocentral-01.azurewebsites.net/products)
- [Order service](https://order-service-lab3-bout0167-cfb7czf5adc6c0bk.mexicocentral-01.azurewebsites.net)
- [Store front](http://158.23.21.14:8080/)

## Github repos:
- [lab3-order-service](https://github.com/bout0167/lab3-order-service.git)
- [lab3-product-service](https://github.com/bout0167/lab3-product-service.git)
- [lab3-store-front](https://github.com/bout0167/lab3-store-front.git)

## Reflections:
### What challenges did you face when configuring environment variables in GitHub Actions?
I had some problems with the Azure connection in GitHub Actions. GitHub could not find my Azure subscription at first. After fixing the Azure settings, the deployment worked.

### What is the difference between Azure Web App and running microservices locally?
Locally, I have to run and manage the services on my own computer. With Azure Web App, the services are hosted and available online through Azure.

### Why are environment variables important in cloud applications?
Environment variables store important settings outside the code. In this lab, they were used to connect the services to RabbitMQ and to connect the store front to the backend services.

## AI disclosure
AI (ChatGPT and Claude) were used to help me understand the lab requirements and simplify the steps.

I encountered a few errors and used AI to help me understand and fix them.

I also used AI to improve the wording and grammar in my README file.

## Demo video
[https://youtu.be/zqPwgXLFdfg](https://youtu.be/zqPwgXLFdfg)
