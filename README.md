# Networking & Concurrency Concepts

## 🔹 Three-Way Handshake (TCP Connection Establishment)

The **three-way handshake** is used in TCP to establish a reliable connection between a client and a server.

1. **SYN** → Client sends a synchronization (SYN) packet to the server, asking to start a connection.
2. **SYN-ACK** → Server responds with a synchronization-acknowledgment (SYN-ACK) packet, acknowledging the request and agreeing to connect.
3. **ACK** → Client replies with an acknowledgment (ACK) packet, confirming the connection is established.

✅ Now the connection is open, and data can be exchanged reliably.

---

## 🔹 Thread Pool

A **thread pool** is a collection of pre-created worker threads that can be reused to execute tasks.  
Instead of creating a new thread for each request (which is expensive), tasks are assigned to idle threads in the pool.

**Advantages:**
- Reduces the overhead of creating/destroying threads repeatedly.
- Efficient use of system resources.
- Improves performance in concurrent systems.

---

## 🔹 Why a Thread Pool is Sufficient?

- Most applications don’t need an unlimited number of threads (too many threads cause **context switching overhead** and **memory usage spikes**).
- A fixed-size thread pool is usually enough to handle the workload efficiently.
- Tasks wait in a **queue** when all threads are busy, ensuring controlled execution.
- It balances **throughput** and **resource usage**, making the system scalable and stable.

---


 # MultiThreaded_Server_ThreadPool and performance analysis using JMeter
 ![image](https://github.com/user-attachments/assets/77dedbe2-4bba-4e7c-941b-4fb2ede0e784)
 result of the requests
![image](https://github.com/user-attachments/assets/840bb810-e419-42ff-89ac-c63541e94ddd)
![image](https://github.com/user-attachments/assets/06f6310b-aba1-4581-8e84-68bb3a3b57cc)




