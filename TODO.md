# TODO - Percorso di Formazione Tech 2026

## DA COMPLETARE

### Modulo 13: System Design
- [ ] Framework per affrontare un problema di system design:
  - [ ] Raccolta requisiti (funzionali e non funzionali)
  - [ ] Back-of-the-envelope estimation (traffico, storage, bandwidth)
  - [ ] API design
  - [ ] Data model e scelta database
  - [ ] High-level design
  - [ ] Deep dive sui componenti critici
- [ ] Esercizi completi:
  - [ ] URL Shortener (hashing, base62, read-heavy system)
  - [ ] Chat System (WebSocket, presence, message delivery)
  - [ ] News Feed / Timeline (fan-out on write vs read, ranking)
  - [ ] Rate Limiter (token bucket, sliding window, distributed)
  - [ ] Notification System (push, email, SMS, priority queue)
- [ ] Pattern ricorrenti:
  - [ ] Database sharding e partitioning strategies
  - [ ] Consistent hashing
  - [ ] Message queue come disaccoppiamento
  - [ ] CDN e caching multi-livello
  - [ ] Database replication (master-slave, multi-master)
- [ ] Quiz interattivo
- [ ] Domande da colloquio

### Modulo 14: Concurrency & Multithreading
- [ ] Fondamenti:
  - [ ] Thread, Runnable, Callable
  - [ ] Thread lifecycle e stati
  - [ ] synchronized, volatile, atomic classes
  - [ ] Race conditions e deadlock (detection, prevention)
- [ ] Java Concurrency API:
  - [ ] ExecutorService e ThreadPool (Fixed, Cached, Scheduled)
  - [ ] Future e CompletableFuture (chaining, combining, error handling)
  - [ ] CountDownLatch, CyclicBarrier, Semaphore
  - [ ] Concurrent Collections (ConcurrentHashMap, BlockingQueue, CopyOnWriteArrayList)
  - [ ] ReadWriteLock vs StampedLock
- [ ] Virtual Threads (Java 21):
  - [ ] Platform threads vs virtual threads
  - [ ] Structured concurrency
  - [ ] Quando usare e quando evitare
- [ ] Pattern:
  - [ ] Producer-Consumer
  - [ ] Thread-safe Singleton
  - [ ] Fork/Join framework
- [ ] Quiz interattivo
- [ ] Domande da colloquio

### Modulo 15: Design Patterns
- [ ] Creational:
  - [ ] Factory Method e Abstract Factory
  - [ ] Builder (con esempi Java reali: Lombok, Stream API)
  - [ ] Singleton (thread-safe, enum, problemi con testing)
  - [ ] Prototype
- [ ] Structural:
  - [ ] Adapter
  - [ ] Decorator (Java I/O streams come esempio)
  - [ ] Facade
  - [ ] Proxy (collegamento con Spring AOP)
- [ ] Behavioral:
  - [ ] Strategy (con lambdas in Java moderno)
  - [ ] Observer (collegamento con event-driven architecture)
  - [ ] Template Method
  - [ ] Chain of Responsibility (middleware, filter chain)
  - [ ] Command
- [ ] Quando usare e quando evitare (anti-pattern di overengineering)
- [ ] Quiz interattivo
- [ ] Domande da colloquio

### Modulo 16: Java Internals & JVM
- [ ] JVM Architecture:
  - [ ] Class loading (Bootstrap, Extension, Application)
  - [ ] Memory model (Heap, Stack, Metaspace, Code Cache)
  - [ ] JIT compilation (C1, C2, Graal)
- [ ] Garbage Collection:
  - [ ] GC roots e reachability
  - [ ] Generational GC (Young, Old, Survivor spaces)
  - [ ] GC algorithms (Serial, Parallel, G1, ZGC, Shenandoah)
  - [ ] GC tuning e flag comuni
  - [ ] Memory leaks: cause e diagnosi
- [ ] Generics deep dive:
  - [ ] Type erasure
  - [ ] Bounded wildcards (PECS: Producer Extends, Consumer Super)
  - [ ] Generic methods
- [ ] Java Records, Sealed Classes, Pattern Matching (Java 17+)
- [ ] Quiz interattivo
- [ ] Domande da colloquio

### Modulo 17: Distributed Systems Avanzati
- [ ] Saga Pattern:
  - [ ] Orchestration vs Choreography (diagrammi, pro/contro)
  - [ ] Compensating transactions
  - [ ] Implementazione con Kafka/eventi
- [ ] Distributed Transactions:
  - [ ] Two-Phase Commit (2PC) e problemi
  - [ ] Outbox Pattern
  - [ ] Change Data Capture (Debezium)
- [ ] Idempotency Patterns:
  - [ ] Idempotency key
  - [ ] Deduplication strategies
  - [ ] At-least-once vs exactly-once delivery
- [ ] Consensus:
  - [ ] Raft (concetti base: leader election, log replication)
  - [ ] Perche' serve (split-brain, network partition)
- [ ] Distributed Locking (Redis Redlock, ZooKeeper)
- [ ] Quiz interattivo
- [ ] Domande da colloquio

### Modulo 18: Coding Patterns Avanzati
- [ ] Dynamic Programming:
  - [ ] Top-down (memoization) vs Bottom-up (tabulation)
  - [ ] Climbing Stairs, Coin Change, Longest Common Subsequence
  - [ ] Knapsack (0/1 e unbounded)
- [ ] Sliding Window:
  - [ ] Fixed vs Variable window
  - [ ] Maximum Subarray Sum, Longest Substring Without Repeating
- [ ] Two Pointers:
  - [ ] Two Sum (sorted), Container With Most Water, 3Sum
- [ ] Backtracking:
  - [ ] Permutations, Combinations, Subsets
  - [ ] N-Queens, Sudoku Solver
- [ ] Binary Search avanzato:
  - [ ] Search in Rotated Array
  - [ ] Find Minimum in Rotated Array
  - [ ] Search range
- [ ] Ogni problema con soluzione Java commentata e analisi complessita'
- [ ] Quiz interattivo
- [ ] Domande da colloquio

---

## Note Tecniche

- **File principale**: `index.html` (HTML5 autosufficiente con CSS e JS inline)
- **Syntax highlighting**: Prism.js via CDN
- **Design**: Dark mode, sidebar navigation, responsive
- **Quiz**: JavaScript con feedback immediato e spiegazioni dettagliate
- **Lingua**: Spiegazioni in italiano, terminologia tecnica in inglese

## Convenzioni Codice

- ID sezioni: `modulo{N}-{topic}` (es: `modulo3-cap-theorem`)
- ID quiz: `q{N}` progressivo globale (ultimo usato: q60)
- Diagrammi: ASCII art dentro `<div class="diagram"><pre>...</pre></div>`
- Info box: `<div class="info-box">`, `.info-box.warning`, `.info-box.success`
