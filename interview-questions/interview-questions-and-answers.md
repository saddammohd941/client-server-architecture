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
