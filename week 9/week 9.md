# Lecture 09: Virtualisation and Cloud


## Context

- Traditional IT used physical, multi-user servers with high costs.
- Developers need flexibility, while production environments require consistency.
- **Virtualisation** provides consistent environments without physical duplication.

---

## What is Virtualisation?

- Splits physical resources into **Virtual Machines (VMs)**.
- A **hypervisor** manages guest machines from a host.
- Guest VMs can run different OSes and share host resources.
- Example use: Testing Linux code on a Windows machine.

---

## Key Technologies

### 1. **VirtualBox**
- Open-source hypervisor.
- Runs VMs with custom operating systems.

### 2. **WSL (Windows Subsystem for Linux)**
- Run Linux (e.g., Ubuntu) directly within Windows.
- Linux apps can behave as native Windows apps.

### 3. **Vagrant**
- Uses **VagrantFile** to script VM setups.
- Enables **Infrastructure as Code**.
- Keeps environments consistent across developers.

---

## Benefits of VMs

- Easily disposable—just delete and recreate.
- Safe testing environments that won’t corrupt your machine.
- Files stay on the host to avoid data loss.
- Use tools like **Puppet** to manage production-scale VMs.

---

## Containerisation

- More lightweight than full VMs.
- Runs isolated apps with shared OS kernel.
- Ideal for microservices and efficient resource usage.

### 4. **Docker**
- Manages containers with isolation.
- Uses **Dockerfile** to define app environments.
- Popular for both local dev and production deployments.

---

## Cloud Computing

- Cloud uses virtualisation to offer computing as a service.
- Provides **Virtual Private Servers (VPS)** and managed container platforms.

### 5. **Cloud Platforms**
- Examples: AWS, Azure, Google Cloud, DigitalOcean.
- Offer services like compute, storage, and networking.

---

## Cloud Economics

- **Pay-As-You-Go (PAYG)**: Pay only for used resources:
  - CPU
  - Disk
  - Network
- ~95% cheaper than buying hardware (per AWS).
- **Benefits**:
  - Scalability
  - Resilience
  - Green computing
  - Global access
  - Lower maintenance

---

## Cloud Service Models

- **IaaS** – Infrastructure as a Service (e.g., virtual servers)
- **PaaS** – Platform as a Service (e.g., app hosting)
- **SaaS** – Software as a Service (e.g., Office 365, Xero)

