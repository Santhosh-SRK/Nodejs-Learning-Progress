# Introduction to Node.js

## 1. What is Node.js?
Node.js is an **open-source**, **cross-platform** JavaScript runtime environment built on Chrome's V8 engine, allowing you to run JavaScript on the server side.

- It has an **event-driven architecture** with **asynchronous I/O**, meaning Node.js can handle multiple operations simultaneously without waiting for one to complete. This makes it highly efficient for I/O-heavy tasks like web servers and APIs.
- Node.js enables you to run JavaScript **outside the browser**, making it ideal for server-side applications.
- **Use Cases**: Node.js is used to create web servers, APIs, real-time applications (like chat apps), and microservices, all thanks to its **performance**, **scalability**, and **efficiency**.
- Node.js is maintained by the **OpenJS Foundation**, ensuring ongoing development and support.
- Node.js helps u run javascript outside web browser.

---

## 2. Why was Node.js created?

Before Node.js, most web servers (like **Apache HTTP Server**) used **blocking I/O**, where each request would block the server from processing other requests until the current one was completed. This made handling multiple concurrent connections inefficient, especially for I/O-heavy tasks.

- The main intention behind creating Node.js was to build a server with **non-blocking I/O**, which allows Node.js to handle multiple requests simultaneously without waiting for one to finish. This makes it much more efficient for **real-time applications** and **high-concurrency** scenarios, like chat apps or APIs.
- Node.js was created to improve **scalability** and **performance** in handling a large number of simultaneous connections, especially in use cases where **latency is important**.

---

## 3. History of Node.js

### 2009:
- **Node.js** was created by **Ryan Dahl**. Initially, SpiderMonkey was chosen as the JavaScript engine, but it was quickly switched to **V8** (the engine used by Google Chrome) because of its superior performance.
- Ryan Dahl was invited by **Joyent** to continue developing Node.js.
- Originally named **Web.js** (indicating its intended use for web servers), the name was changed to **Node.js** to reflect its broader use case.

### 2010:
- **npm** (Node Package Manager) was created by **Isaac Schlueter**, becoming integral to Node.js, making it easier for developers to install and manage packages or libraries.

### 2011:
- **Windows support** was added to Node.js, which originally supported only **Linux** and **macOS**.

### 2012:
- **Ryan Dahl** left the Node.js project, and **Isaac Schlueter** became the new project lead.

### 2014:
- **io.js** was introduced as a fork of Node.js with a focus on faster releases and a more open, community-driven governance model.

### 2015:
- The **Node.js Foundation** was founded, and the codebases of Node.js and io.js were merged into one unified project.

### 2019:
- The **JS Foundation** and **Node.js Foundation** merged to form the **OpenJS Foundation**, which fosters collaboration in the JavaScript ecosystem.

---

## What is NPM?

**NPM (Node Package Manager)** is the default package manager for Node.js, used to install, share, and manage dependencies (libraries or packages) for JavaScript and Node.js projects.

- NPM was created to address the need for managing packages and their dependencies in a consistent and efficient manner.

While npm is the standard, **Yarn** and **pnpm** are popular alternative package managers that aim to offer faster and more efficient package management.

---

## How NPM Works

- **package.json**: This file holds metadata for your project, including the list of dependencies (external libraries) needed for the project.
- **package-lock.json**: This file records the exact version of each installed package to ensure consistency across environments.

---

## How to Install Dependencies Using NPM:

1. To install a specific package, run:
   ```bash
   npm i <package-name>

# difference between npm,yarn,pnpm

| Feature               | **npm**                              | **Yarn**                            | **pnpm**                           |
|-----------------------|--------------------------------------|-------------------------------------|------------------------------------|
| **Installation Speed** | Slower, single-threaded             | Faster, parallel installs           | Very fast, optimized disk usage   |
| **Lock File**          | `package-lock.json`                 | `yarn.lock`                         | `pnpm-lock.yaml`                  |
| **Disk Space Efficiency** | Less optimized                    | More efficient than npm             | Highly efficient, uses a global store |
| **Popularity**         | Most widely used, default           | Popular in Facebook/React           | Gaining popularity, especially for monorepos |
