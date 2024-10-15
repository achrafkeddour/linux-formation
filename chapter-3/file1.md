## Applications and the Kernel

The **kernel** acts as an air traffic controller, managing system resources and applications (airplanes) .

### Resource Management
- Applications request resources like memory, CPU, and disk space. (from kernel) 
- The kernel allocates resources and may kill applications to prevent system crashes.

### Abstraction of Details
- Applications interact with hardware through the kernel’s API, without worrying about specific hardware details.
- The kernel manages memory, creating an illusion of a large, continuous block for each application.

### Multitasking
- The kernel switches between tasks (multitasking) to efficiently use limited CPUs and memory.
- It pauses tasks when necessary to allow other tasks to run.

### Processes
- Applications are broken down into **processes**, which the kernel runs, tracks, and manages. 
