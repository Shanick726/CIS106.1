# Notes Lecture 02
### What is Virtualization?
* Creating a "fake" computer inside of your pc.
* Two general types of virtualization.
  * Server-side virtualization.
  * Client-side virtualization. 
      * Difference is where the virtualization takes place.
  ### Server-Side Virtualization.
**Virtual Desktop Infrastructure (VDI)**
* Thin Client or Fat client
* Thin client
* Zero client
  ### Client-side virualization.
 * Softwar installed to manage Virtual Machine VM.
 * each VM has its own opp system.
 * For client side virtualization, Comp needs:
    * A hypervisor (software that allows management of VM)
    * Hardware support
  * capable CPU
  * Enough RAM
  * Enough storage
  ### Type 1 VS Type 2 Hypervisor
  **Type 1**
  Runs on hardware
    EX) VMware ESX & ESXi
**Type 2**
Runs on Hosting Operating System
    EX) Oracle VirtualBox
  ![img1](notes2img1.PNG)
  ### VirtualBox
  * Powerful type 2 virtualization product for enterprise as well as home use.
  * Open source software under GPL version 2
  * Supports large number of guest operating systems.
  ### Installing Ubuntu 20.04
  * Name virtual machine
    * Name w/ use of VM
  * Select a memory size 
    * Requires at least 2GB of RAM
  * If you wish Create Hard disc
    * allows to create a virtual hard disk w/ any size
  * Choose type of file you would like to use for the new hard dick
    * Virtual disk image format.
  * Choose storage you would like to use.
    * Select Dynamically allocated.
  * Choose file location size
    * Ubuntu takes about 25GB of disc space.
  ### What is a Raspberry Pi
  The raspberry Pi is a low cost, credit-card sized computer that plugs into a computer monitor or tv, and uses a standard keyboard and mouse. It is capable of doing everything you'd expect a desktop computer to do.
