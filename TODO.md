# TODO - Manuale Definitivo per Colloqui Tecnici 2026

## Stato Avanzamento

### COMPLETATI

- [x] **Modulo 1: Java & Spring Boot Deep Dive**
  - [x] Inversion of Control & Dependency Injection
  - [x] Bean Lifecycle (diagramma completo 9 fasi)
  - [x] Spring Annotations (tutte le principali categorie)
  - [x] Proxy Pattern (JDK vs CGLIB, self-invocation)
  - [x] @Transactional (propagation, isolation, rollback)
  - [x] Spring Security (OAuth2/JWT)
  - [x] Spring Data JPA & N+1 Problem
  - [x] Quiz interattivo (5 domande)

- [x] **Modulo 2: Testing Strategy**
  - [x] Test Pyramid (diagramma, anti-pattern Ice Cream Cone)
  - [x] Unit vs Integration vs E2E Tests (esempi con JUnit, Mockito, TestContainers, REST Assured)
  - [x] Mocking vs Stubbing (taxonomy test doubles)
  - [x] Quiz interattivo (4 domande)
  - [x] ~~TDD~~ (rimosso su richiesta utente)

- [x] **Modulo 3: Architettura & Scalabilità**
  - [x] Monoliti vs Microservizi (pro/contro, Modular Monolith)
  - [x] Pattern di resilienza:
    - [x] Circuit Breaker (stati: closed, open, half-open) con Resilience4j
    - [x] Bulkhead Pattern (semaphore e thread-pool)
    - [x] Retry Pattern con Exponential Backoff
    - [x] Timeout Pattern
  - [x] CAP Theorem (+ PACELC, consistency models)
  - [x] Load Balancing (Round Robin, Least Connections, Weighted, Consistent Hashing, L4 vs L7)
  - [x] Caching strategies (Cache-Aside, Write-Through, Write-Behind, Redis vs Memcached)
  - [x] Quiz interattivo (5 domande, q11-q15)

- [x] **Modulo 4: Database & Messaging**
  - [x] SQL vs NoSQL (ACID vs BASE, polyglot persistence, quando usare)
  - [x] Deep dive Kafka:
    - [x] Event streaming architecture (topics, partitions, brokers)
    - [x] Partitions, Consumer Groups, offsets
    - [x] Exactly-once semantics (idempotent producer, transactions)
    - [x] Partitioning strategy
  - [x] Deep dive RabbitMQ:
    - [x] Message broker concepts (AMQP)
    - [x] Exchange types (Direct, Fanout, Topic, Headers)
    - [x] Queues, Bindings, DLQ
    - [x] Acknowledgments e retry
  - [x] Kafka vs RabbitMQ (tabella comparativa, when to use what)
  - [x] Quiz interattivo (5 domande, q16-q20)

- [x] **Modulo 5: Cloud & DevOps**
  - [x] Docker (Containerization):
    - [x] Container vs VM (diagramma comparativo)
    - [x] Dockerfile best practices
    - [x] Multi-stage builds
    - [x] Layer caching (diagramma cache invalidation)
    - [x] Docker Compose per sviluppo locale
  - [x] Kubernetes:
    - [x] Architettura cluster (Control Plane, Worker Nodes)
    - [x] Pod (resources, probes, env)
    - [x] Deployment (rolling update strategy)
    - [x] Service (ClusterIP, NodePort, LoadBalancer, ExternalName)
    - [x] Ingress (TLS, routing rules)
    - [x] ConfigMaps e Secrets
    - [x] Horizontal Pod Autoscaler (HPA)
  - [x] CI/CD Pipelines:
    - [x] GitHub Actions (workflow completo con test, build, deploy)
    - [x] Jenkins (Declarative Pipeline con Jenkinsfile)
    - [x] Confronto GitHub Actions vs Jenkins
  - [x] Deployment strategies:
    - [x] Rolling Update (diagramma progressivo)
    - [x] Blue-Green (diagramma switch, rollback istantaneo)
    - [x] Canary (diagramma fasi, Argo Rollouts, AnalysisTemplate)
    - [x] Tabella comparativa strategie
  - [x] Quiz interattivo (5 domande, q21-q25)

- [x] **Modulo 6: Advanced Topics 2026**
  - [x] Observability:
    - [x] I tre pilastri (Logs, Metrics, Traces)
    - [x] Logging (structured logging, MDC, ELK stack, Loki)
    - [x] Metrics (Prometheus, Micrometer, PromQL, Four Golden Signals)
    - [x] Tracing (OpenTelemetry, Jaeger, Context Propagation, Sampling)
    - [x] Correlazione tra i tre pilastri
  - [x] Infrastructure as Code:
    - [x] Terraform basics (HCL, providers, resources, data sources)
    - [x] Terraform workflow (init, plan, apply, destroy)
    - [x] State management (remote state, locking, security)
    - [x] Modules (riusabilità, Terraform Registry)
    - [x] Best practices
  - [x] LLM/AI Integration:
    - [x] RAG (Retrieval Augmented Generation) architecture
    - [x] Embeddings e similarity search
    - [x] Vector Databases (Pinecone, Weaviate, pgvector, Milvus, Qdrant)
    - [x] Spring AI implementation
    - [x] Advanced patterns (Hybrid Search, Query Transformation, Chunking)
    - [x] Considerazioni architetturali (latency, cost, security)
  - [x] Quiz interattivo (5 domande, q26-q30)
  - [x] Domande da colloquio (7 domande con risposte)

- [x] **Modulo 7: Coding Challenges**
  - [x] LRU Cache:
    - [x] Approccio HashMap + Doubly Linked List (diagramma)
    - [x] Soluzione commentata Java
    - [x] Soluzione commentata Python (con OrderedDict)
    - [x] Analisi complessità O(1) get/put
    - [x] Errori comuni da evitare
  - [x] Valid Parentheses:
    - [x] Approccio Stack (diagramma step-by-step)
    - [x] Soluzione commentata Java (due versioni)
    - [x] Soluzione commentata Python
    - [x] Analisi complessità O(n) time, O(n) space
    - [x] Varianti del problema
  - [x] Merge Intervals:
    - [x] Approccio Sort + Linear Scan (diagramma)
    - [x] Soluzione commentata Java
    - [x] Soluzione commentata Python
    - [x] Analisi complessità O(n log n)
    - [x] Varianti del problema
  - [x] Quiz interattivo (5 domande, q31-q35)
  - [x] Domande da colloquio (6 domande con risposte)

- [x] **Modulo 8: Paradigmi di Programmazione**
  - [x] Programmazione Funzionale:
    - [x] Pure Functions (con esempi Java)
    - [x] Immutability (record Java, vantaggi)
    - [x] First-Class Functions (Function, closure)
    - [x] Higher-order functions (map, filter, reduce con diagramma)
  - [x] Java Streams API:
    - [x] Stream vs Collection
    - [x] Operazioni Intermediate vs Terminal
    - [x] Esempi completi (filter, map, flatMap, groupingBy, etc.)
    - [x] Optional e null-safety (anti-pattern)
    - [x] Parallel Streams (quando usare)
  - [x] Confronto OOP vs FP:
    - [x] Tabella comparativa
    - [x] Quando usare cosa (diagramma decisionale)
    - [x] Esempio pratico stesso problema in entrambi gli stili
    - [x] Composizione di funzioni
    - [x] Pattern funzionali (currying, memoization, Either)
  - [x] Quiz interattivo (5 domande, q36-q40)
  - [x] Domande da colloquio (6 domande con risposte)

---

## Note Tecniche

- **File principale**: `index.html` (HTML5 autosufficiente con CSS e JS inline)
- **Syntax highlighting**: Prism.js via CDN
- **Design**: Dark mode, sidebar navigation, responsive
- **Quiz**: JavaScript con feedback immediato e spiegazioni dettagliate
- **Lingua**: Spiegazioni in italiano, terminologia tecnica in inglese

## Come Riprendere

1. Aprire `index.html` e cercare l'ultimo modulo completato
2. Aggiungere link nella sidebar per il nuovo modulo
3. Aggiungere contenuto prima di `</main>`
4. Aggiungere spiegazioni quiz nell'oggetto `explanations` nel JavaScript
5. Aggiornare questo TODO.md

## Convenzioni Codice

- ID sezioni: `modulo{N}-{topic}` (es: `modulo3-cap-theorem`)
- ID quiz: `q{N}` progressivo globale (ultimo usato: q40)
- Diagrammi: ASCII art dentro `<div class="diagram"><pre>...</pre></div>`
- Info box: `<div class="info-box">`, `.info-box.warning`, `.info-box.success`
