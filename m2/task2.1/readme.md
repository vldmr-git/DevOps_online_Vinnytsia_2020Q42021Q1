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
1. Acquainted with the [VirtualBox user manual](https://www.virtualbox.org/manual/UserManual.html)  
2. Downloaded and installed the [VirtualBox-6.1.16-140961-Win.exe](https://download.virtualbox.org/virtualbox/6.1.16/VirtualBox-6.1.16-140961-Win.exe)  
3. Created VM1 and installed Ubuntu on it:  
![Creating of VM1](/m2/task2.1/img/Screenshot1.3.png)  
4. Acquainted with the possibilities of VM1 control:  
![VM1 controls](/m2/task2.1/img/Screenshot1.4.png)  
5. Cloned an existing VM1 and created VM2:  
![Cloning](/m2/task2.1/img/Screenshot1.5.png)  
6. Created a group of two VM: VM1, VM2:  
![Creating](/m2/task2.1/img/Screenshot1.6.png)  
7. Took several different snapshots:  
![Snapshots](/m2/task2.1/img/Screenshot1.7.png)  
8. Saved \*.ova file to disk and imported VM from this \*.ova file:  
![Export/Import](/m2/task2.1/img/Screenshot1.8.png)  

#### 2. Configuration of virtual machines  
1. Explored VM configuration options:  
![Conf options](/m2/task2.1/img/Screenshot2.1.png)  
2. Configured the USB to connect the USB ports of the host machine:  
![Conf the USB](/m2/task2.1/img/Screenshot2.2.png)  
3. Configured a shared folder between VM and host:  
![Conf shared folder](/m2/task2.1/img/Screenshot2.3.png)  
4. Configured different network modes:  

<table>
	<tr>	
		<td>Mode</td><td>VM -> Host</td><td>VM <- Host</td><td>VM1 <-> VM2</td><td>VM -> Net/LAN</td><td>VM -> Net/LAN</td>
	</tr>
	<tr>
		<td>Host-only</td><td>+</td><td>+</td><td>+</td><td>-</td><td>-</td>
	</tr>
	<tr>
		<td>Internal</td><td>-</td><td>-</td><td>+</td><td>-</td><td>-</td>
	</tr>
	<tr>
		<td>Bridged</td><td>+</td><td>+</td><td>+</td><td>+</td><td>+</td>
	</tr>
	<tr>
		<td>NAT</td><td>+</td><td><a href="https://www.virtualbox.org/manual/UserManual.html#natforward">Port forward</a></td><td>-</td><td>+</td><td><a href="https://www.virtualbox.org/manual/UserManual.html#natforward">Port forward</a></td>
	</tr>
	<tr>
		<td>NATservice</td><td>+</td><td><a href="https://www.virtualbox.org/manual/UserManual.html#network_nat_service">Port forward</a></td><td>+</td><td>+</td><td><a href="https://www.virtualbox.org/manual/UserManual.html#network_nat_service">Port forward</a></td>
	</tr>
</table>  

#### 3. Work with CLI through VBoxManage.  
1. Have run the cmd.exe command line:  
![Work with CLI](/m2/task2.1/img/Screenshot3.png)  
2. Acquainted with the purpose of the VBoxManage basic commands:  
`showvminfo`, `createvm`, `startvm`, `modifyvm`, `clonevm`, `snapshot`, `controlvm`.  

### PART 3. WORK WITH VAGRANT  
1. Downloaded the required version of [Vagrant](https://releases.hashicorp.com/vagrant/2.2.14/vagrant_2.2.14_x86_64.msi).  
And checked the path to Vagrant:  
![Path to vagrant](/m2/task2.1/img/Screenshot3.1.png)  
2. Have run the powershell and created the folder "vmstangrit":  
![Creating folder](/m2/task2.1/img/Screenshot3.2.png)  
3. Initialized the environment with the default Vagrant box:  
![Initialization](/m2/task2.1/img/Screenshot3.3.png)  
4. Have run `vagrant up`:  
![Vagrant up](/m2/task2.1/img/Screenshot3.4.png)  
5. Connected to the VM using the PuTTY using SSH:  
![Connecting VM](/m2/task2.1/img/Screenshot3.5.png)  
6. Recorded the date using `date` command:  
![Date](/m2/task2.1/img/Screenshot3.6.png)  
7. Stoped and deleted the VM:  
![Stoped and deleted the VM](/m2/task2.1/img/Screenshot3.7.png)  
8. 