## Chapter 2: Exchanges

Exchanges are simply put routers in a RabbitMQ broker. They are used to rout messages to the specified (bounded) queues. They route the messages based on a specific routing key. A queue cannot be created without binding it to a certain exchange. Even the simplest queue creation (where you do not declaratively specify an exchange) must be bound to an exchange that has routing key as the name of the queue itself.

There are four types of exchanges:
1. Direct Exchanges
2. Fanout Exchanges
3. Topic Exchanges
4. Header Exchanges

We will look at each one separately with an code example written in C# using <a href="https://www.rabbitmq.com/dotnet.html" target="_blank">RabbitMQ .NET Client library</a>.

### 2.1 Direct Exchanges

* Definition and explanation 
* Simple exchange with one queue (Image and code)
* Worker consumers on one queue (Image and code)
* 2 consumers on separate queues with specific routing key used in the exchange
 (Image and code)

### 2.2 Fanout Exchanges (Broadcast)

* Definition and explanation 
* One exchange with multiple queues message copy (Image and code)

### 2.3 Topic Exchanges (Multicast)

* Definition and explanation 
* One exchange with multiple queues with different routing keys with wildcards (Image and code)

### 2.4 Header Exchanges

Header exchanges

### 2.5 RPC (Rmote Procedure Call)

Image and code example