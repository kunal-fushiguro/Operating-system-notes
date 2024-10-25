# Operating system

Operating system is an interface between computer hardware and user. The purpose of an operating system is to provide an environment in which a user can execute programs conveniently and efficiently.

## Key points

- operating system is the one program running at all times on the computer (usually called the kernel).
- provide appropriate mechanisms to ensure the correct operation of the computer system and to prevent user programs from interfering with the proper operation of the system.

## Characteristics

- **Resource and Device Management**: Manages devices, files, memory, and processors, allocating resources efficiently and controlling system performance.

- **Security and Reliability**: Protects data and programs from unauthorized access, detects errors, and provides debugging tools.

- **User Convenience and Efficiency**: Enhances ease of use, optimizes resource utilization, and maintains high throughput.

- **Adaptability and Scalability**: Supports system evolution, allowing new features to be developed and integrated without disrupting existing services.

## Components of an Operating System

**Shell** : The shell is a program that acts as an interface between the user and the kernel.

**kernel** : The kernel is the core of the OS and is responsible for controlling all system-related tasks. there are four types of kernel : Monolithic Kernel, Microkernel , Hybrid Kernel , Exokernel

## Difference Between 32-Bit and 64-Bit Operating Systems

| 32-Bit Operating System                                                                                          | 64-Bit Operating System                                                                 |
| ---------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| 32-Bit OS is required for running of 32-Bit Processors, as they are not capable of running on 64-bit processors. | 64-Bit Processors can run on any of the Operating Systems, like 32-Bit OS or 64-Bit OS. |
| 32-Bit OS gives a low efficient performance.                                                                     | 64-Bit Operating System provides highly efficient Performance.                          |
| Less amount of data is managed in 32-Bit Operating System as compared to 64-Bit Os.                              | A large amount of data can be stored in 64-Bit Operating System.                        |
| 32-Bit Operating System can address 2^32 bytes of RAM.                                                           | 64-Bit Operating System can address 2^64 bytes of RAM.                                  |

## Functions of an Operating System

### Memory Management

- **Memory Tracking**: The OS monitors memory usage, keeping track of allocated and free memory addresses for various processes.
- **Access Management**: In multiprogramming, the OS determines the order and duration of memory access for processes.
- **Memory Allocation**: The OS allocates memory to a process upon request and deallocates it when the process terminates or performs I/O operations.
- **Protection**: The OS ensures that processes do not access memory allocated to other processes, maintaining data integrity and security.

### Processor Management

- **Process Scheduling**: The OS determines the order and time allocation for processes to access the CPU in a multiprogramming environment.

- **Job Allocation**: The OS allocates jobs to the processor, ensuring each process receives adequate processing time to operate effectively.

- **Process Status Tracking**: The OS monitors the status of processes, functioning like a traffic controller to manage their execution.

- **CPU Management**: The OS allocates the CPU to processes and deallocates it when a process completes or is no longer needed.

### Device Management

- **Device Tracking**: The OS keeps track of all connected devices and assigns an Input/Output controller for each device.

- **Access Management**: The OS decides which process can access a device and for how long.

- **Device Allocation**: The OS allocates devices efficiently and deallocates them when they are no longer needed.

- **Communication Handling**: The OS manages communication with input/output devices, processing requests and relaying responses to the requesting processes.

### File Management

- **File Tracking and Management**: The OS keeps track of file information, including creation, deletion, transfer, and storage, while managing user access settings and file status.

- **Data Integrity and Security**: The OS maintains the integrity of stored data and the file directory structure, protecting against unauthorized access.

### Network Management

- **Data Packaging and Transmission**: The OS manages how data is packaged and sent over the network, ensuring it arrives safely and in the correct order.

- **Network Configuration and Monitoring**: The OS allows users to set up network connections (like Wi-Fi or Ethernet) and monitors network performance for efficiency and security.

### User Interface or Command Interpreter

- The operating system acts as an interface between the user and computer hardware, enabling interaction through command-line inputs or a graphical user interface (GUI).

### Booting the Computer

- Booting is starting a computer; cold booting is powering it on from off, while warm booting restarts it via the operating system.

### Security

- The operating system employs password protection and firewalls to prevent unauthorized access and ensure data integrity.
- It safeguards system memory from malicious access and alerts users about potential vulnerabilities.

### Control Over System Performance

- Operating systems optimize system performance by managing resource allocation and process scheduling to ensure efficient use of CPU, memory, and I/O devices.

### Job Accounting

- The operating system monitors resource usage and manages task scheduling to allocate time to applications in a multitasking environment.

### Error-Detecting Aids

- The operating system monitors for errors, external threats, and hardware damage, providing alerts for necessary user actions.

### Coordination Between Other Software and Users

- The operating system acts like a traffic cop, coordinating software usage and managing resources to ensure smooth operation without conflicts.

## Types of Operating Systems

### Batch Operating System

Groups similar jobs for efficient processing without user interaction.

- **Advantages**: Efficient resource use, low idle time.
- **Disadvantages**: Difficult to debug, unpredictable job wait times.

### Multi-Programming Operating System

Allows multiple programs in memory for better resource utilization.

- **Advantages**: Increased throughput, reduced response time.
- **Disadvantages**: Limited user interaction.

### Multi-Processing Operating System

Utilizes multiple CPUs for resource execution.

- **Advantages**: Increased throughput, fault tolerance.
- **Disadvantages**: Complexity in management.

### Multi-Tasking Operating System

Runs multiple programs simultaneously using scheduling algorithms.

- **Advantages**: Concurrent execution, efficient memory management.
- **Disadvantages**: Potential overheating under heavy load.

### Time-Sharing Operating System

Allocates CPU time to multiple tasks for smooth operation.

- **Advantages**: Equal opportunity for tasks, improved productivity.
- **Disadvantages**: Higher overhead, security risks.

### Distributed Operating System

Connects multiple autonomous systems for shared resources.

- **Advantages**: Independent systems, scalable.
- **Disadvantages**: Network failure impacts communication, high complexity.

### Network Operating System

Manages data and resources over a network, allowing shared access.

- **Advantages**: Centralized security, remote access.
- **Disadvantages**: Costly servers, dependency on central location.

### Real-Time Operating System

Processes inputs with strict time constraints for critical applications.

- **Advantages**: High resource utilization, quick task shifting.
- **Disadvantages**: Limited simultaneous tasks, complex algorithms.

## Computer Boot Process

- **Power Supply Activation** : When the computer is turned on, the power supply sends electricity to essential components like the motherboard, hard drive, and fans.

- **BIOS Initialization** : The Basic Input/Output System (BIOS) performs a Power-On Self-Test (POST) to check the functionality of hardware components (CPU, RAM, video card, etc.). If issues are detected, error messages or beep codes are displayed.

- **Master Boot Record (MBR)** : After POST, the BIOS locates the Master Boot Record on the boot disk, which contains the boot loader code necessary to load the operating system.

- **Boot Loader Activation** : The boot loader is loaded into memory and executed, initiating the loading of the operating system (OS) into RAM.

- **Operating System Initialization** : The OS initializes its components and drivers, eventually presenting the user with a login screen or desktop environment.

- **Run Levels and Init** : The `init` process determines the initial run level of the system, which defines its operational state (e.g., single user mode, multi-user mode). It also starts necessary daemons for networking and services, including the X server for graphical interface management.

- **System Configuration** : The BIOS allows users to configure settings such as boot order, system time, and hardware parameters (CPU voltage, clock speed).

- **Security Features** : The BIOS may include security measures like password protection, secure boot (to prevent unauthorized software), and Trusted Platform Module (TPM) for hardware-based security and encryption.
