# Systems & Software Engineering Portfolio

**Yiyang Liu | Computer Science & Mathematics @ University of Maryland**

This repository contains selected systems programming, algorithms, and software engineering projects that demonstrate my work with **Java, C, x86-64 Assembly, memory management, concurrency, data structures, and performance optimization**.

For my current professional and full-stack work, including **OrkaOS**, **SEO Master Tracker**, and **Sustainable Earth**, visit my [GitHub profile](https://github.com/Lanny76).

> **Source Code Notice:** Some projects in this repository were completed as part of university coursework. To comply with academic integrity policies, source code is not publicly available. Demos, technical explanations, and implementation details are included where possible, and I can discuss my work in greater depth during interviews.

---

## 🎮 BlockDrop — 2D Game Engine

**Java · AWT/Swing · Object-Oriented Design · Coordinate Geometry**

A collaborative real-time puzzle game in which I focused on the core game engine: object behavior, collision detection, transformations, and game-state logic.

### What I Built

* **Collision System**
  Implemented four-direction collision handling for left, right, bottom, and stacked interactions using a 2D representation of the game board.

* **Piece Rotation**
  Applied coordinate transformations to support 90° clockwise rotations around dynamically calculated anchor points.

* **Game-State Logic**
  Developed special game mechanics that monitor score and board state to trigger new behaviors and piece types.

* **Rendering Separation**
  Separated logical board coordinates from screen rendering so game behavior remained independent of display positioning and frame rate.

### Engineering Focus

This project gave me experience designing software where several systems must interact reliably in real time. I worked extensively with object-oriented architecture, geometric reasoning, state transitions, and debugging complex interactions between moving pieces and the game board.

### Demo

[▶ Watch the BlockDrop Demo](https://github.com/Lanny76/Engineering-Portfolio/blob/main/assets/BlockDrop%202025-03-11%2021-58-38.mp4)

---

## ⚙️ High-Performance Memory & Matrix Engine

**C · x86-64 Assembly · pthreads · mmap · GDB · Valgrind**

A collection of lower-level systems programming projects focused on understanding how software interacts with memory, operating-system primitives, CPU caches, and multiple processor cores.

### Custom Memory Allocator — `el_malloc`

Implemented a custom dynamic memory allocator as an alternative to the standard C `malloc`.

#### Key Components

* Requested heap memory directly from the operating system using `mmap`
* Managed allocated and free regions using a **doubly linked list of memory blocks**
* Used manual pointer arithmetic to navigate block metadata and memory boundaries
* Split larger free blocks when servicing smaller allocation requests
* Implemented **block coalescing** to merge neighboring free regions
* Debugged memory behavior using **GDB** and **Valgrind**

### What I Learned

Building an allocator required reasoning about memory layout at a much lower level than normal application development. It strengthened my understanding of pointers, heap organization, fragmentation, metadata management, and the relationship between a program and the operating system.

---

### Cache-Aware Matrix Operations

Implemented and optimized matrix-processing algorithms with a focus on CPU performance.

#### Optimization Work

* Reorganized memory-access patterns to improve **spatial locality**
* Reduced unnecessary cache misses during matrix traversal
* Compared alternative loop and data-access structures to understand their effect on performance
* Analyzed how algorithmic decisions interact with the CPU memory hierarchy

This project reinforced that performance depends not only on asymptotic complexity, but also on how programs actually interact with hardware.

---

### Multithreaded Matrix Computation

Used **POSIX Threads (`pthreads`)** to parallelize computationally expensive matrix operations.

* Divided work across multiple threads
* Coordinated workloads across CPU cores
* Evaluated the relationship between parallelism and execution time
* Worked with synchronization and thread-management primitives in C

---

## 📊 C Data Visualizer

**C · Algorithms · Data Processing · Visualization**

A data-driven C application for analyzing historical financial data and translating numerical results into visual output.

### What I Built

* Parsed structured financial datasets into internal data representations
* Implemented algorithms for identifying favorable historical buy and sell windows
* Converted numerical values into graphical coordinates
* Handled scaling and offsets when mapping raw data into a visual representation
* Combined data analysis and rendering logic in a low-level C environment

### Engineering Focus

This project explored the connection between **data representation, algorithmic analysis, and visualization** without relying on a high-level visualization framework.

---

## 🧠 Areas Demonstrated

Across these projects, I worked with:

* Manual memory management
* Pointer arithmetic
* Data structures
* Heap organization and fragmentation
* Multithreading and concurrency
* CPU cache behavior
* Performance optimization
* Object-oriented architecture
* Collision detection
* Coordinate transformations
* State-based game logic
* Data parsing and visualization
* Debugging with GDB and Valgrind

---

## 🌐 Looking for My Current Work?

My newer projects include production web development, automation, full-stack applications, and technical SEO.

* **[OrkaOS](https://github.com/PROJXON/OrkaOS)** — Production React product website
* **[SEO Master Tracker](https://github.com/PROJXON/seo-master-tracker)** — Automated Python SEO monitoring and auditing
* **[Sustainable Earth](https://github.com/Lanny76/SustainableEarth)** — Award-winning full-stack eco-finance application
* **[GitHub Profile](https://github.com/Lanny76)** — Full overview of my experience and featured work

---

## 📫 Connect

* [LinkedIn](https://www.linkedin.com/in/yiyang-liu-umd/)
* [GitHub](https://github.com/Lanny76)
* **Email:** [yiyangliu254@gmail.com](mailto:yiyangliu254@gmail.com)
