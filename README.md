# System Design from Scratch - FANG Interview Preparation

## 1. Understand the Problem Statement
- Clarify functional and non-functional requirements.
- Identify constraints (number of users, data size, latency, etc.).
- Ask clarifying questions (e.g., read-heavy or write-heavy system?).

---

## 2. Define High-Level Architecture
- Choose architecture style: Monolithic, Microservices, Event-Driven, Serverless.
- Identify core components (e.g., API Gateway, Load Balancer, Databases, Caching).

### Example Architecture:
- **Client** → **Load Balancer** → **Web Servers** → **Application Layer** → **Database**.
- Use **CDN** for static content.
- Implement **caching** (Redis, Memcached) for frequently accessed data.

---

## 3. Database Design
- Choose the right database type: SQL (PostgreSQL, MySQL) vs. NoSQL (MongoDB, Cassandra).
- Design **data schema** and **indexing strategies**.
- Optimize for **sharding** and **replication** to improve performance.
- Consider **eventual consistency** vs. **strong consistency** trade-offs.

---

## 4. Scalability Considerations
- **Vertical scaling (Scale-Up)**: Increase server resources.
- **Horizontal scaling (Scale-Out)**: Distribute load across multiple servers.
- Use **Load Balancers (Nginx, HAProxy, AWS ALB)**.
- Implement **database sharding** for handling high traffic.

---

## 5. Caching Strategies
- **Client-side caching** (Browser cache, Service Workers).
- **CDN (Content Delivery Network)** for serving static files (Cloudflare, AWS CloudFront).
- **Database caching** (Read replicas, Redis, Memcached).
- **Application-layer caching** for frequently accessed API responses.

---

## 6. Data Partitioning and Replication
- **Replication**: Master-Slave, Multi-Master, or Leader-Follower models.
- **Sharding**: Range-based, Hash-based, Directory-based sharding.
- Ensure data consistency using **CAP Theorem** (Consistency, Availability, Partition Tolerance).

---

## 7. API Design and Communication
- Use **RESTful APIs** or **GraphQL** for efficient data fetching.
- Implement **gRPC** or **WebSockets** for real-time communication.
- Use **Rate Limiting (API Gateway, Nginx, Cloudflare)** to prevent abuse.

---

## 8. Message Queues and Event Processing
- Use **Kafka, RabbitMQ, AWS SQS** for asynchronous processing.
- Implement **event-driven architecture** for scalability (Pub-Sub model).
- Ensure **idempotency** for safe retries.

---

## 9. Security Considerations
- **Authentication**: JWT, OAuth 2.0, OpenID.
- **Authorization**: Role-based access control (RBAC).
- **Data encryption**: TLS for transit, AES for storage.
- **DDoS protection**: WAF (Web Application Firewall), Rate limiting.
- **Input validation**: Prevent SQL Injection, XSS, CSRF.

---

## 10. Logging, Monitoring & Observability
- Use **ELK Stack (Elasticsearch, Logstash, Kibana)** for logging.
- Implement **Distributed Tracing (Jaeger, OpenTelemetry)**.
- Set up **alerting** with Prometheus and Grafana.
- Monitor application performance with **APM tools (New Relic, Datadog)**.

---

## 11. Failover and Disaster Recovery
- **Multi-region deployment** for high availability.
- **Auto-scaling** using Kubernetes, AWS Autoscaling Groups.
- **Database backups** and **disaster recovery plans**.

---

## 12. Deployment and CI/CD
- **Infrastructure as Code (Terraform, CloudFormation)**.
- **Containerization (Docker, Kubernetes)**.
- **CI/CD Pipelines (Jenkins, GitHub Actions, GitLab CI)**.

---

## Example System Designs for FANG Interviews
1. **URL Shortener** (Bit.ly)
2. **Rate Limiter** (API Gateway)
3. **Distributed Cache System** (Like Redis)
4. **Design Twitter/Instagram Feed**
5. **Real-time Chat System** (WhatsApp, Slack)
6. **Ride-Sharing System** (Uber, Lyft)
7. **E-Commerce Platform** (Amazon, Flipkart)
8. **File Storage System** (Google Drive, Dropbox)
9. **Video Streaming System** (YouTube, Netflix)

---

## How to Use This Guide?
- Study each section in depth.
- Practice designing systems with a whiteboard.
- Optimize and iterate on your designs based on feedback.
- Mock system design interviews with peers.

---

🚀 **Happy Learning and Good Luck with Your FANG Interviews!**

