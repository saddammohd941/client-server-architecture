# 🧩 **Client-Server Architecture – Questions with Answers & Explanations**

---

### 🔸 **1. What is client-server architecture?**

* **Answer:** It’s a computing model where the client requests services and the server provides them.
* **Explanation:** This design separates concerns — clients handle UI; servers handle logic/data.

---

### 🔸 **2. How is a client different from a server?**

* **Answer:** A client initiates requests; a server waits for and processes them.
* **Explanation:** Clients are consumers, servers are providers.

---

### 🔸 **3. What are the key components of a client-server system?**

* **Answer:** Client, Server, Network, Protocols (e.g., HTTP, TCP/IP).
* **Explanation:** Each part handles a specific layer of communication and data exchange.

---

### 🔸 **4. What is a stateless server?**

* **Answer:** A server that does not retain session information between requests.
* **Explanation:** Common in REST APIs, improves scalability.

---

### 🔸 **5. What’s the difference between 2-tier and 3-tier architecture?**

* **Answer:** 2-tier: client ↔ DB server; 3-tier: client ↔ app server ↔ DB.
* **Explanation:** 3-tier adds a middle (application) layer for better separation and scalability.

---

### 🔸 **6. What is the role of a reverse proxy in client-server architecture?**

* **Answer:** Forwards client requests to backend servers, can load balance and cache.
* **Explanation:** Acts as an intermediary to optimize performance and security.

---

### 🔸 **7. Give examples of common client-server applications.**

* **Answer:** Web browsers (client) + web servers, FTP clients + FTP servers, email clients + SMTP/IMAP servers.
* **Explanation:** The model is widely used in internet services.

---

### 🔸 **8. What is an API in the context of client-server?**

* **Answer:** A set of endpoints clients use to interact with server functionality.
* **Explanation:** APIs are the interface layer of modern distributed systems.

---

### 🔸 **9. What protocols are typically used in client-server communication?**

* **Answer:** HTTP/HTTPS, FTP, SMTP, IMAP, SSH, TCP/IP.
* **Explanation:** Protocols define how data is formatted and transmitted.

---

### 🔸 **10. What is session management in a client-server system?**

* **Answer:** Maintaining user context (login status, cart data) across multiple requests.
* **Explanation:** Sessions can be stored in memory, files, databases, or tokens.

---

### 🔸 **11. How does load balancing improve client-server systems?**

* **Answer:** Distributes requests across multiple servers to prevent overload.
* **Explanation:** Improves availability, scalability, and fault tolerance.

---

### 🔸 **12. What is a thin client?**

* **Answer:** A minimal device that relies heavily on the server for processing.
* **Explanation:** Used in environments like VDI or Citrix.

---

### 🔸 **13. What is a socket?**

* **Answer:** An endpoint for communication between client and server over a network.
* **Explanation:** TCP/IP communication uses sockets.

---

### 🔸 **14. How does DNS fit into client-server architecture?**

* **Answer:** Resolves domain names (like `google.com`) to IP addresses for clients.
* **Explanation:** It's the starting point of most web client-server communications.

---

### 🔸 **15. What is the difference between synchronous and asynchronous client-server communication?**

* **Answer:** Sync: client waits for a response. Async: client continues without waiting.
* **Explanation:** Async improves performance in modern apps (AJAX, REST with callbacks).

---

### 🔸 **16. What is middleware in client-server architecture?**

* **Answer:** Software that connects client and server apps, handling communication and logic.
* **Explanation:** Examples include message brokers, API gateways, or application servers.

---

### 🔸 **17. What are the pros and cons of client-server architecture?**

* **Answer:** Pros: centralized control, easier maintenance. Cons: server can be a bottleneck.
* **Explanation:** Design must balance performance and complexity.

---

### 🔸 **18. How can a server handle multiple client requests at once?**

* **Answer:** Using multithreading, forking, event loops, or async I/O.
* **Explanation:** Efficient concurrency is key in high-load systems.

---

### 🔸 **19. How do firewalls impact client-server architecture?**

* **Answer:** They filter traffic, which can block or allow client-server communication.
* **Explanation:** Network rules must be configured correctly for access.

---

### 🔸 **20. What is TLS/SSL in client-server communication?**

* **Answer:** Encryption protocols that secure data between client and server.
* **Explanation:** HTTPS uses SSL/TLS to protect web data in transit.

---

### 🔸 **21. Describe a typical web request lifecycle.**

* **Answer:** Client sends HTTP request → DNS resolution → server processes → response sent.
* **Explanation:** Understanding this helps troubleshoot latency or errors.

---

### 🔸 **22. What is connection pooling?**

* **Answer:** Reusing established connections instead of creating new ones.
* **Explanation:** Reduces latency and resource overhead for repeated client requests.

---

### 🔸 **23. What is a client timeout?**

* **Answer:** The time a client waits for a server response before aborting.
* **Explanation:** Prevents clients from hanging on long or failed requests.

---

### 🔸 **24. How can caching improve client-server performance?**

* **Answer:** Stores frequent responses to reduce load and response time.
* **Explanation:** Done on client (browser), CDN, or server side.

---

### 🔸 **25. What is REST and how does it fit client-server model?**

* **Answer:** REST is an API style that uses HTTP for stateless communication.
* **Explanation:** It decouples clients and servers for flexible, scalable design.

---

### 🔸 **26. What’s the purpose of authentication in client-server systems?**

* **Answer:** Verifies client identity before granting access.
* **Explanation:** Common methods: tokens, OAuth, JWT.

---

### 🔸 **27. What is NAT and how does it affect client-server connections?**

* **Answer:** Network Address Translation hides internal IPs behind a public IP.
* **Explanation:** May require port forwarding for external client access.

---

### 🔸 **28. What is a microservice client-server interaction model?**

* **Answer:** Each service is a mini server; clients (often other services) consume APIs.
* **Explanation:** Promotes modular, scalable system design.

---

### 🔸 **29. In a failover scenario, how does a client reconnect to another server?**

* **Answer:** Via DNS failover, service discovery, or load balancers.
* **Explanation:** Enables high availability and disaster recovery.

---

### 🔸 **30. How do you simulate multiple client connections to test a server?**

* **Answer:** Use tools like `ab`, `wrk`, `JMeter`, or custom scripts with `curl`/sockets.
* **Explanation:** Load testing ensures server capacity under stress.

---

### 🔸 **31. A client can ping the server, but cannot connect via SSH. What could be wrong?**

* **Answer:** SSH port (22) may be blocked by a firewall or SSH service not running.
* **Explanation:** Ping uses ICMP, while SSH uses TCP port 22. Different layers.

---

### 🔸 **32. A client can connect to a server, but file transfers are very slow. What do you check?**

* **Answer:** Check network latency (`ping`), bandwidth (`iperf`), and MTU mismatches.
* **Explanation:** High latency, congestion, or duplex mismatches can throttle performance.

---

### 🔸 **33. How does DNS caching affect client-server communication?**

* **Answer:** Cached entries may point to outdated or incorrect IPs.
* **Explanation:** Could cause clients to connect to the wrong or dead server.

---

### 🔸 **34. How would you secure client-server communication over an untrusted network?**

* **Answer:** Use SSH, TLS/SSL, VPN, or IPsec.
* **Explanation:** Encryption ensures confidentiality and integrity of data in transit.

---

### 🔸 **35. What are keep-alive connections and how do they help?**

* **Answer:** Persistent connections that allow multiple requests/responses over a single TCP connection.
* **Explanation:** Reduces connection overhead and latency for HTTP clients.

---

### 🔸 **36. How can you design a client-server system to handle 1 million concurrent users?**

* **Answer:** Use load balancing, horizontal scaling, async servers (e.g., Nginx), and message queues.
* **Explanation:** Scale stateless services, optimize I/O, and distribute load efficiently.

---

### 🔸 **37. A client app fails to connect during DNS failover. What's your approach?**

* **Answer:** Check DNS TTL, client-side DNS caching, or lack of retry logic.
* **Explanation:** Failover depends on how quickly DNS changes propagate and are respected.

---

### 🔸 **38. A client can connect but gets intermittent "timeout" errors. What tools help debug?**

* **Answer:** Use `tcpdump`, `wireshark`, or server logs to trace the flow.
* **Explanation:** Might be due to load spikes, packet loss, or poor timeout settings.

---

### 🔸 **39. Why should a server-side app avoid storing session state in memory?**

* **Answer:** In-memory state doesn’t persist across crashes or multiple servers.
* **Explanation:** Use shared session stores like Redis or databases in distributed systems.

---

### 🔸 **40. A mobile app client must work in spotty networks. How do you adapt the architecture?**

* **Answer:** Use caching, retry queues, sync schedulers, and offline support.
* **Explanation:** Design for "eventual consistency" and degraded network experience.

---

### 🔸 **41. What’s the purpose of heartbeats in client-server communication?**

* **Answer:** Regular signals to check connectivity or keep a session alive.
* **Explanation:** Used in WebSockets, message brokers, and monitoring.

---

### 🔸 **42. A WebSocket connection drops after some time. What might cause this?**

* **Answer:** Idle timeout on firewall, reverse proxy, or server config.
* **Explanation:** Ensure proper keep-alive and timeout settings on all layers.

---

### 🔸 **43. What are sticky sessions in load balancing?**

* **Answer:** Sessions are tied to one server for consistency.
* **Explanation:** Useful when session state is stored locally, but reduces flexibility.

---

### 🔸 **44. Explain how a CDN fits into a client-server architecture.**

* **Answer:** CDNs cache and deliver content closer to the client.
* **Explanation:** Offloads servers and reduces latency for static assets.

---

### 🔸 **45. You see many half-open connections on the server. What's the cause and fix?**

* **Answer:** Could be SYN flood attack. Use SYN cookies or increase backlog in `sysctl`.
* **Explanation:** Protects the TCP handshake stage from being overloaded.

---

### 🔸 **46. How does client-side rendering vs. server-side rendering impact client-server load?**

* **Answer:** Client-side shifts work to the client; server-side increases server load.
* **Explanation:** SSR improves SEO; CSR is more scalable with good caching.

---

### 🔸 **47. What are idempotent operations in client-server systems?**

* **Answer:** Operations that produce the same result if repeated.
* **Explanation:** GET, PUT are idempotent. POST is not. Important for retry logic.

---

### 🔸 **48. Your app uses API calls to a third-party server that’s rate-limited. How do you handle it?**

* **Answer:** Implement rate limiting, exponential backoff, and retries on the client.
* **Explanation:** Prevents getting blocked and handles burst traffic gracefully.

---

### 🔸 **49. How would you design a client-server chat system (like Slack)?**

* **Answer:** Use WebSockets for real-time messaging, with a backend using pub/sub or queues.
* **Explanation:** Requires bi-directional communication, low latency, and message persistence.

---

### 🔸 **50. What is service discovery in client-server architecture (especially microservices)?**

* **Answer:** Automatic detection of services (e.g., via Consul, etcd, or DNS).
* **Explanation:** Clients don't need to know server IPs — discovery abstracts that.

---

### 🔸 **51. What is middleware’s role in client-server architecture?**

* **Answer:** Middleware acts as a communication layer that facilitates interaction between client and server applications.
* **Explanation:** It can handle data translation, message queuing, and service orchestration.

---

### 🔸 **52. What is the difference between thick and thin clients?**

* **Answer:** Thick clients handle more processing locally; thin clients depend mostly on the server for processing.
* **Explanation:** Thick clients can work offline better but require more resources.

---

### 🔸 **53. What is a stateful server?**

* **Answer:** A server that keeps track of client session information across multiple requests.
* **Explanation:** Useful for applications requiring session persistence but harder to scale.

---

### 🔸 **54. How does session persistence (sticky sessions) affect scalability?**

* **Answer:** It limits load balancing flexibility since clients must always connect to the same server.
* **Explanation:** This can cause uneven load distribution.

---

### 🔸 **55. What’s the purpose of load balancers in client-server systems?**

* **Answer:** To distribute incoming client requests evenly across multiple servers.
* **Explanation:** Ensures no single server becomes a bottleneck.

---

### 🔸 **56. How does DNS help in client-server communication?**

* **Answer:** DNS translates human-readable hostnames into IP addresses so clients can locate servers.
* **Explanation:** Without DNS, clients would need to know numeric IPs.

---

### 🔸 **57. What is the difference between synchronous and asynchronous communication?**

* **Answer:** Synchronous requires the client to wait for a server response; asynchronous lets the client continue immediately.
* **Explanation:** Async is better for responsiveness and scalability.

---

### 🔸 **58. What happens during a client-server handshake?**

* **Answer:** Initial connection setup where client and server agree on communication parameters and authentication.
* **Explanation:** Examples include TCP’s three-way handshake or TLS negotiation.

---

### 🔸 **59. What is Remote Procedure Call (RPC)?**

* **Answer:** A protocol that allows a program to execute procedures on a remote server as if they were local.
* **Explanation:** Simplifies remote interactions.

---

### 🔸 **60. What are the pros and cons of TCP vs UDP in client-server apps?**

* **Answer:** TCP is reliable and ordered; UDP is faster but unreliable.
* **Explanation:** Use TCP for data integrity, UDP for speed-sensitive apps like video streaming.

---

### 🔸 **61. What is an API Gateway’s role?**

* **Answer:** It acts as a single entry point, managing authentication, routing, and throttling for API calls.
* **Explanation:** Simplifies client interaction with complex backend services.

---

### 🔸 **62. What does scalability mean in client-server systems?**

* **Answer:** The ability to handle increased load by adding resources.
* **Explanation:** Achieved by scaling vertically (stronger server) or horizontally (more servers).

---

### 🔸 **63. What is multi-tier architecture?**

* **Answer:** A design dividing client-server functions into layers like presentation, logic, and data storage.
* **Explanation:** Improves separation of concerns and maintainability.

---

### 🔸 **64. What’s the difference between polling and push?**

* **Answer:** Polling clients repeatedly check for updates; push servers send updates when available.
* **Explanation:** Push is more efficient for real-time data.

---

### 🔸 **65. How do cookies help maintain client-server state?**

* **Answer:** They store small pieces of data on the client to track sessions and preferences.
* **Explanation:** Essential for session continuity in HTTP’s stateless protocol.

---

### 🔸 **66. Why are stateless servers easier to scale?**

* **Answer:** They don’t keep client data, so any server can handle any request.
* **Explanation:** Simplifies load balancing and failure recovery.

---

### 🔸 **67. What is HTTPS and why is it important?**

* **Answer:** HTTPS encrypts HTTP traffic using SSL/TLS to secure data.
* **Explanation:** Prevents eavesdropping and data tampering.

---

### 🔸 **68. How do WebSockets improve client-server communication?**

* **Answer:** They establish full-duplex, persistent connections allowing real-time data exchange.
* **Explanation:** Useful for chat apps, live updates, gaming.

---

### 🔸 **69. What is service discovery in client-server systems?**

* **Answer:** Automatic detection and connection to available services.
* **Explanation:** Crucial for dynamic environments like microservices.

---

### 🔸 **70. How does caching enhance client-server performance?**

* **Answer:** By storing copies of frequently accessed data closer to clients or servers.
* **Explanation:** Reduces latency and server load.

---

### 🔸 **71. What is throttling in server management?**

* **Answer:** Limiting the rate of requests to prevent abuse or overload.
* **Explanation:** Protects server stability and fair resource distribution.

---

### 🔸 **72. What is a proxy server?**

* **Answer:** An intermediary that forwards requests from clients to servers.
* **Explanation:** Can provide anonymity, caching, or filtering.

---

### 🔸 **73. How do RESTful APIs work in client-server?**

* **Answer:** REST uses stateless HTTP methods to manipulate resources via URLs.
* **Explanation:** Encourages scalability and simplicity.

---

### 🔸 **74. How does SOAP differ from REST?**

* **Answer:** SOAP is protocol-heavy with XML envelopes; REST is lightweight, using standard HTTP.
* **Explanation:** SOAP suits enterprise needs; REST suits web services.

---

### 🔸 **75. What is failover?**

* **Answer:** Automatically switching to backup servers on failure.
* **Explanation:** Ensures continuous service availability.

---

### 🔸 **76. How do firewalls affect client-server communication?**

* **Answer:** Firewalls block or allow traffic based on security policies.
* **Explanation:** Can restrict access and protect from attacks.

---

### 🔸 **77. What are sockets in networking?**

* **Answer:** Endpoints for sending and receiving data over networks.
* **Explanation:** Abstract communication details for apps.

---

### 🔸 **78. What is a port?**

* **Answer:** A numeric identifier for services on a server.
* **Explanation:** Allows multiple services on one IP.

---

### 🔸 **79. What are heartbeat messages?**

* **Answer:** Regular signals to check if a connection or service is alive.
* **Explanation:** Helps detect failures quickly.

---

### 🔸 **80. How does peer-to-peer differ from client-server?**

* **Answer:** P2P is decentralized; clients and servers are the same nodes.
* **Explanation:** Good for resource sharing, but less centralized control.

---

### 🔸 **81. How to secure client-server communication?**

* **Answer:** Use encryption (TLS/SSL), authentication, and authorization.
* **Explanation:** Protects data confidentiality and access control.

---

### 🔸 **82. What is NAT and its impact on client-server?**

* **Answer:** NAT maps private IPs to a public IP, hiding internal networks.
* **Explanation:** May complicate direct server access.

---

### 🔸 **83. How do firewalls and NAT affect server accessibility?**

* **Answer:** Firewalls filter traffic; NAT hides addresses, requiring port forwarding for access.
* **Explanation:** Important for hosting services behind routers.

---

### 🔸 **84. What are SSL certificates?**

* **Answer:** Digital certificates that verify server identity and enable encryption.
* **Explanation:** Builds trust between client and server.

---

### 🔸 **85. What is a reverse proxy?**

* **Answer:** A proxy that forwards requests from clients to backend servers.
* **Explanation:** Used for load balancing, SSL termination, caching.

---

### 🔸 **86. How does client-server differ in cloud environments?**

* **Answer:** Servers are virtualized and scalable on-demand.
* **Explanation:** Enables elasticity and resilience.

---

### 🔸 **87. What is microservices architecture?**

* **Answer:** A collection of small, independent services communicating over networks.
* **Explanation:** Improves modularity and scalability.

---

### 🔸 **88. What is API rate limiting?**

* **Answer:** Controlling the number of API calls clients can make in a time frame.
* **Explanation:** Prevents abuse and ensures fair usage.

---

### 🔸 **89. What is a load balancer health check?**

* **Answer:** Monitoring backend servers to route traffic only to healthy instances.
* **Explanation:** Maintains service reliability.

---

### 🔸 **90. What is a Content Delivery Network (CDN)?**

* **Answer:** Distributed servers that cache and serve content closer to users.
* **Explanation:** Reduces latency and server load.

---

### 🔸 **91. What is a socket timeout?**

* **Answer:** The time a socket waits for data before closing.
* **Explanation:** Prevents hanging connections.

---

### 🔸 **92. What is a handshake protocol?**

* **Answer:** The initial negotiation to establish communication parameters.
* **Explanation:** Ensures secure, agreed-upon communication.

---

### 🔸 **93. How to handle concurrency in client-server apps?**

* **Answer:** Use threads, async I/O, or event loops to serve multiple clients simultaneously.
* **Explanation:** Increases throughput and responsiveness.

---

### 🔸 **94. What is a middleware queue?**

* **Answer:** A message queue that decouples client and server for asynchronous processing.
* **Explanation:** Improves reliability and scalability.

---

### 🔸 **95. What are WebSockets vs HTTP requests?**

* **Answer:** WebSockets provide persistent full-duplex connections; HTTP is request-response.
* **Explanation:** WebSockets better for real-time apps.

---

### 🔸 **96. What is a service mesh?**

* **Answer:** Infrastructure layer managing service-to-service communication in microservices.
* **Explanation:** Handles routing, security, and observability.

---

### 🔸 **97. What is latency in client-server communication?**

* **Answer:** Delay between sending a request and receiving a response.
* **Explanation:** Lower latency means faster user experience.

---

### 🔸 **98. How do asynchronous APIs benefit clients?**

* **Answer:** Clients don’t wait for server response and can continue other work.
* **Explanation:** Improves UI responsiveness.

---

### 🔸 **99. What is an edge server?**

* **Answer:** Server located close to clients to deliver faster content.
* **Explanation:** Often part of a CDN.

---

### 🔸 **100. How do you monitor a client-server system?**

* **Answer:** Using logging, metrics, alerts, and tracing tools like Prometheus or ELK stack.
* **Explanation:** Helps detect issues and optimize performance.

---