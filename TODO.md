# TODO - Percorso di Formazione Tech 2026

## DA COMPLETARE

### Modulo 13: System Design ✅
- [x] Framework per affrontare un problema di system design:
  - [x] Raccolta requisiti (funzionali e non funzionali)
  - [x] Back-of-the-envelope estimation (traffico, storage, bandwidth)
  - [x] API design
  - [x] Data model e scelta database
  - [x] High-level design
  - [x] Deep dive sui componenti critici
- [x] Esercizi completi:
  - [x] URL Shortener (hashing, base62, read-heavy system)
  - [x] Chat System (WebSocket, presence, message delivery)
  - [x] News Feed / Timeline (fan-out on write vs read, ranking)
  - [x] Rate Limiter (token bucket, sliding window, distributed)
  - [x] Notification System (push, email, SMS, priority queue)
- [x] Pattern ricorrenti:
  - [x] Database sharding e partitioning strategies
  - [x] Consistent hashing
  - [x] Message queue come disaccoppiamento
  - [x] CDN e caching multi-livello
  - [x] Database replication (master-slave, multi-master)
- [x] Quiz interattivo
- [x] Domande da colloquio

### Modulo 14: Concurrency & Multithreading ✅
- [x] Fondamenti:
  - [x] Thread, Runnable, Callable
  - [x] Thread lifecycle e stati
  - [x] synchronized, volatile, atomic classes
  - [x] Race conditions e deadlock (detection, prevention)
- [x] Java Concurrency API:
  - [x] ExecutorService e ThreadPool (Fixed, Cached, Scheduled)
  - [x] Future e CompletableFuture (chaining, combining, error handling)
  - [x] CountDownLatch, CyclicBarrier, Semaphore
  - [x] Concurrent Collections (ConcurrentHashMap, BlockingQueue, CopyOnWriteArrayList)
  - [x] ReadWriteLock vs StampedLock
- [x] Virtual Threads (Java 21):
  - [x] Platform threads vs virtual threads
  - [x] Structured concurrency
  - [x] Quando usare e quando evitare
- [x] Pattern:
  - [x] Producer-Consumer
  - [x] Thread-safe Singleton
  - [x] Fork/Join framework
- [x] Quiz interattivo
- [x] Domande da colloquio

### Modulo 15: Design Patterns ✅
- [x] Creational:
  - [x] Factory Method e Abstract Factory
  - [x] Builder (con esempi Java reali: Lombok, Stream API)
  - [x] Singleton (thread-safe, enum, problemi con testing)
  - [x] Prototype
- [x] Structural:
  - [x] Adapter
  - [x] Decorator (Java I/O streams come esempio)
  - [x] Facade
  - [x] Proxy (collegamento con Spring AOP)
- [x] Behavioral:
  - [x] Strategy (con lambdas in Java moderno)
  - [x] Observer (collegamento con event-driven architecture)
  - [x] Template Method
  - [x] Chain of Responsibility (middleware, filter chain)
  - [x] Command
- [x] Quando usare e quando evitare (anti-pattern di overengineering)
- [x] Quiz interattivo
- [x] Domande da colloquio

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
- ID quiz: `q{N}` progressivo globale (ultimo usato: q70)
- Diagrammi: ASCII art dentro `<div class="diagram"><pre>...</pre></div>`
- Info box: `<div class="info-box">`, `.info-box.warning`, `.info-box.success`
