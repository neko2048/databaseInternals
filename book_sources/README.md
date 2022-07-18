# Database Internals A Deep Dive Into How Distributed Data Systems Work
## Preface

### Scaling:
* Horizontal Scaling (scaling out) - 
    improving performance by running more instances (更多員工)
* Vertical scaling (scaling in) - 
    move to a powerful machine (找更有能力的員工)

### Structure of This book:
How the database system <font color="#e6b422">stored</font> and how they <font color="#e6b422">distribute</font> the data
* Part I - Store
    1. architecture of a database management system.
    2. Ways to classify the database system by the [primary storage medium](https://www.computerhope.com/jargon/p/primstor.htm) and layout.
    3. how disk-based structures are different from in-memory ones.
    4. B-Tree and algorithms for efficiently maintaining B-Tree.
    5. Variants to illustrate the power of [4] and the diversity of data structure influenced and inspired by B-Tree.
    6. Varients of log-structured storage.
* Part II - Distribution
    * How to organize multiple nodes into a database cluster
        1. The importance of building fault-tolerance distributed systems.
        2. How distributed systems are different from single-node applications. (problems, constraints, and complications)
    * Algorithms for failure detection
