# Operating Systems
Modern operating systems do more than just manage hardware and software. 

1. They allow **multiple programs** to run at the same time by sharing the computer’s processor, making it seem like everything happens simultaneously. 
2. They also **provide services** that let users and programs request tasks, like printing a document. If the request is made correctly, the operating system will perform the function needed.

The term **operating system** applies to any **software that is booted and controls a device**, whether it's a basic set-top box or a powerful supercomputer.

---
# Specifying Computer Systems

## 1. **Role**
- **Desktop**: 
  - Used directly by a user.
  - Runs productivity applications, web browsing.
  - Graphical User Interface (GUI) is preferred for ease of use.
  
- **Server**: 
  - Accessed remotely by users or systems (clients).
  - Provides services remotely.
  - Often runs Command Line Interface (CLI) for better resource management. (liberer les ressources)
  - Typically located in a rack and accessed via shared keyboard/monitor.

## 2. **Function** 
- Identify the software or functions the machine must support.
- Determine the scale (hundreds or thousands of machines).
- Consider the skill level of the team managing the system.

## 3. **Life Cycle**
- **Release Cycle**: Periodic updates for operating systems and software.
- **Maintenance Cycle**: Time during which the vendor supports older versions.
- In enterprise settings, upgrading software is expensive, so servers are often replaced for performance gains.

### Example:
- **ubuntu Linux 102.04** is in the **release cycle** until **ubuntu Linux 104.04** comes out.
- **ubuntu Linux 102.04** stays in the **maintenance cycle** as long as the maintainers provide updates, and once support ends, it reaches **end of life**.
  
## 4. **Considerations for Upgrades**
- **Virtualization**: 
  - One physical machine hosts multiple virtual machines (VMs), reducing physical space, power needs, and allowing automation.
  - VMs can be created and managed with scripting.
  
- **Cloud Services**:
  - Providers like AWS, Rackspace, and Azure reduce the need for frequent hardware upgrades.

## 5. **Stability**
- **Beta Software**: 
  - Has new features, not fully tested. 
  - Used during development to test and request new features.
  
- **Stable Software**: 
  - Fully tested, typically used in production environments.
  
- **Open Source**: 
  - Early releases for peer review and feedback.  
  - Fast iteration with community support.
  
- **Proprietary Software**: 
  - Developed in secrecy, reaches beta later in the process.

## 6. **Compatibility**
- **Backward Compatibility**: 
  - Ensures newer OS versions can run software designed for older versions.
  - Open source projects prioritize maintaining compatibility.
  
- **Versioning**: 
  - Libraries are versioned to maintain older functionality while introducing new features.

## 7. **Cost**
- **Licensing Fees**: 
  - Companies like Microsoft charge annual fees for servers, software, and users.
  
- **Virtualization & Outsourcing**: 
  - Pay only for what is used (e.g., cloud services).
  - Reduces upfront costs and helps control long-term expenses.
  
---

> sid : the unstable branch of debian operating system 
