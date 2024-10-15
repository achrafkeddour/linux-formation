### 3.2 Applications

The kernel of the operating system is like an **air traffic controller** at an airport, and the applications are the airplanes under its control. The kernel:
- Decides which program gets which blocks of memory.
- Starts and kills applications.
- Handles displaying text or graphics on a monitor.

#### Resource Management
Applications make requests to the kernel and in return receive resources, such as:
- Memory
- CPU
- Disk space

If two applications request the same resource, the kernel decides which one gets it, and in some cases, kills off one application to save the rest of the system and prevent a crash.

#### Abstraction of Details
The kernel abstracts away complicated details. For example:
- An application doesn’t need to know if a block of disk storage is on a **solid-state drive**, **hard disk**, or even a **network file share**.
- Applications interact with the kernel through an **Application Programming Interface (API)** without worrying about hardware implementation details.

Each application behaves as if it has a large block of memory. The kernel maintains this illusion by:
- Remapping smaller blocks of memory.
- Sharing blocks of memory with other applications.
- Swapping out untouched blocks to disk.

#### Multitasking
The kernel handles the switching of applications in a process known as **multitasking**. A computer system has a limited number of **CPUs** and finite **memory**. The kernel manages this by:
- Unloading one task and loading a new one if there is more demand than resources.
- Pausing a task when it has run for a specified time so that another task can run.
- Switching between tasks rapidly, creating the illusion that the computer is doing many things at once.

#### Processes
When we think of applications, we usually think of **word processors**, **web browsers**, or **email clients**. However, there are many types of applications. 

The kernel doesn’t differentiate between:
- User-facing applications.
- Network services that communicate with remote computers.
- Internal system tasks.

This leads to the concept of a **process**. A process is a single task that is loaded and tracked by the kernel. Some applications may need multiple processes to function. The kernel:
- Runs these processes.
- Starts and stops them as requested.
- Manages the allocation of system resources to them.
