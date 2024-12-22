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


Azure Service Bus is a fully managed enterprise message broker that provides reliable messaging services. Its primary components—**queues, topics, and subscriptions**—enable asynchronous communication and support different messaging patterns, such as **point-to-point** and **publish-subscribe**.

---

### **1. Queues: Point-to-Point Communication**
   - **Concept**: Queues enable **one-to-one** communication between a single sender and a single receiver.
   - **How It Works**:
     - A sender sends messages to the queue.
     - A receiver retrieves messages from the queue.
     - Each message is processed by a single consumer.
   - **Key Features**:
     - **FIFO (First In, First Out)**: Messages are processed in the order they arrive.
     - **Durable Messaging**: Messages are stored until they are consumed or expire.
     - **Load Balancing**: Multiple receivers can compete for messages, distributing the workload.

---

### **2. Topics and Subscriptions: Publish-Subscribe Communication**
   - **Concept**: Topics enable **one-to-many** communication, where a message is delivered to multiple subscribers.
   - **How It Works**:
     - A sender sends messages to a **topic**.
     - Each **subscription** under the topic receives a copy of the message.
     - Subscribers can define filters to receive only specific messages.
   - **Key Features**:
     - **Decoupling**: Publishers and subscribers are independent.
     - **Message Filtering**: Use SQL-like filters to route messages to specific subscriptions.
     - **Fan-Out**: A single message can be delivered to multiple subscriptions.

---

### **Key Differences Between Queues and Topics**
| Feature                  | Queues                             | Topics and Subscriptions           |
|--------------------------|-------------------------------------|-------------------------------------|
| Communication Pattern    | Point-to-point                     | Publish-subscribe                  |
| Number of Receivers      | Single receiver per message         | Multiple receivers via subscriptions|
| Message Delivery         | One-to-one                         | One-to-many                        |
| Message Filtering        | Not available                      | Supported through filters          |

---

### **Use Cases**
- **Queues**:
  - Task scheduling where each task is processed by a single worker.
  - Order processing systems where each order is handled by one service.
  
- **Topics and Subscriptions**:
  - Notification systems where multiple services need to respond to the same event.
  - Logging systems where logs are sent to multiple consumers for processing and storage.

---

### **Advanced Features**
1. **Dead Letter Queues (DLQs)**:
   - Used to store messages that cannot be delivered or processed.
   - Applicable to both queues and topic subscriptions.

2. **Message Sessions**:
   - Enables FIFO delivery with session-aware processing.

3. **Auto Forwarding**:
   - Allows chaining of queues or topics for advanced routing scenarios.

4. **Message TTL (Time-To-Live)**:
   - Specifies how long a message should remain in the queue or topic.

---

By leveraging these concepts, Azure Service Bus provides a robust solution for decoupling applications, enabling scalable and fault-tolerant message-driven architectures.