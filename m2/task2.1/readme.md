# readme.md  
## Task2.1  

### PART1. HYPERVISORS  
1. The most popular hypervisors for infrustructure virtualization are:  
- VMware vSphere Hypervisor  
- Microsoft Hyper-V  
- Citrix XenServer  
- Oracle VirtualBox  
- Red Hat Enterprise Virtualization Hypervisor (REVH)  
- KVM
- Parallels
- Qemu  
2. The main difference of the most popular hypervisors:  
- Type 1 hypervisors, **native or bare-metal hypervisors**.  
	> They runs directly on the host's hardware to control the hardware and to manage guest operating systems.  
	> - Microsoft Hyper-V  
	> - VMware ESX Server  
	> - Citrix XenServer  
- Type 2 hypervisors, **hosted hypervisors**.  
	> - They runs on a conventional operating system (OS) just as other computer programs do. A guest operating system runs as a process on the host.
	> - VMware Workstation  
	> - Oracle VirtualBox
	> - Microsoft Virtual PC  
	> - Parallels Desktop  
	> - QEMU  

### PART2. WORK WITH VIRTUALBOX  
#### 1. First run VirtualBox and Virtual Machine (VM).  
1. Acquainted with  the [VirtualBox user manual](https://www.virtualbox.org/manual/UserManual.html)  
2. Downloaded and installed the [VirtualBox-6.1.16-140961-Win.exe](https://download.virtualbox.org/virtualbox/6.1.16/VirtualBox-6.1.16-140961-Win.exe)  
3. Created VM1 and installed Ubuntu on it
![Creating of VM1](/m2/task2.1/img/Screenshot1.3.png)  
4. Acquainted with the possibilities of VM1 control  
![VM1 controls](/m2/task2.1/img/Screenshot1.4.png)  
5. Cloned an existing VM1 and created VM2  
![Cloning](/m2/task2.1/img/Screenshot1.5.png)  
6. Created a group of two VM: VM1, VM2  
![Creating](/m2/task2.1/img/Screenshot1.6.png)  
7. Took several different snapshots  
![Snapshots](/m2/task2.1/img/Screenshot1.7.png)  
8. Saved \*.ova file to disk and imported VM from this \*.ova file  
![Export/Import](/m2/task2.1/img/Screenshot1.8.png)  

#### 2. Configuration of virtual machines  
1. Explored VM configuration options.  
![Conf options](/m2/task2.1/img/Screenshot2.1.png)  
2. 