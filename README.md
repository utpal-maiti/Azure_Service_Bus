### Azure Service Bus

Guidance:
https://microsoftlearning.github.io/AZ-204-DevelopingSolutionsforMicrosoftAzure/Instructions/Labs/AZ-204_lab_10.html
Solution:
https://github.com/utpal-maiti/AZ-204-DevelopingSolutionsforMicrosoftAzure/tree/master/Allfiles/Labs/09/Solution/

**Azure Service Bus** is a fully managed enterprise message broker that facilitates reliable and secure messaging between applications and services. It supports various messaging patterns, including **queues**, **topics**, and **subscriptions**, making it ideal for decoupling applications and improving scalability and reliability.

### Key Features of Azure Service Bus

1. **Queues**: Implement **First In, First Out (FIFO)** message delivery to one or more competing consumers. Messages are stored durably and processed in the order they were added.
2. **Topics and Subscriptions**: Enable **publish-subscribe** messaging patterns, allowing multiple subscribers to receive messages from a single topic.
3. **Reliable Messaging**: Ensure messages are delivered even when the receiving application is offline.
4. **Scalability**: Automatically scale to handle varying loads and ensure high availability.
5. **Security**: Built-in security features, including encryption, authentication, and authorization.
6. **Integration**: Seamlessly integrates with other Azure services and supports hybrid solutions.

### Common Use Cases

- **Decoupling Applications**: Improve the reliability and scalability of applications by decoupling components.
- **Load Balancing**: Distribute workloads across multiple consumers to handle traffic spikes.
- **Event-Driven Architectures**: Build event-driven applications that respond to state changes in real-time.
- **Enterprise Messaging**: Facilitate communication between different parts of an enterprise system.

### Getting Started with Azure Service Bus

1. **Create a Service Bus Namespace**: Use the Azure portal, CLI, or ARM templates to create a new namespace.
2. **Create Messaging Entities**: Create queues, topics, and subscriptions within your namespace.
3. **Send and Receive Messages**: Use the Service Bus APIs or SDKs to send and receive messages from your queues and topics.
4. **Monitor and Manage**: Use Azure Monitor and Azure Security Center to track and manage your Service Bus resources.
