---
permalink: LINKS/
---
# LINKS

## Week 00 - 01: Setting up with M1

1. [UTM](https://mac.getutm.app/)<br>

  UTM is an alternative to VirtualBox that runs on the Apple Silicon Chip (M1). Our fantastic lecturer Pak RMS
  has kindly prepared [an in-depth tutorial](https://doit.vlsm.org/009.html) on how to setup a Debian VM with UTM.

2. [FileZilla](https://filezilla-project.org/)<br>

  FileZilla is an FTP client like WinSCP, except of course WinSCP is not available on MacOS. FileZilla functions 
  almost identically to WinSCP, though you may first need to run the Configuration Wizard under `Settings > FTP > Overview`. Make sure passive mode is
  prioritized and enable your external IP address if given the option.

3. [Bash in 100 Seconds](https://youtu.be/I4EWvMFj37g)<br>

  Being a Mac M1 user has exactly one benefit in the Operating Systems course: familiarity with Bash (or Bash-based, like Zsh) scripting languages. The       video linked is not exactly a tutorial but it gives a pretty neat big-picture view of it. Bash is ESSENTIAL to making the most use of Linux (and Mac, to   an extent) so don't hesitate to search for more in-depth Bash guides.
  
## Week 02: Getting Settled

1. [RegexOne](https://regexone.com/)<br>

  Where to start with Regex? This website provides step-by-step lessons for understanding Regex while still giving you freedom to experiment with it along the way.

2. [What is a Checksum?](https://www.howtogeek.com/363735/what-is-a-checksum-and-why-should-you-care/)<br> 
  
  After doing the Week 02 assignments, you may have questions about the SHA checksum and myscript.sh. I know I did, but fortunately this page along with Pak RMS' thorough explanation had made clear what exactly  myscript.sh does.

3. Intro to C:  [Tutorialspoint](https://www.tutorialspoint.com/cprogramming/index.htm) and [JavaTPoint](https://www.javatpoint.com/c-programming-language-tutorial)

  The two links above are excellent complements to Week 02's C Programming Demos.

## Week 03: File Systems

1. [UIC OS Course Notes](https://www.cs.uic.edu/~jbell/CourseNotes/OperatingSystems/)

  I found this while trying to learn about File Systems. This page contains a concise summary of each chapter from Silberschatz's OSC textbook, eighth edition. Do note that the edition difference means not everything is up-to-date.

2. [tldr.sh](https://tldr.sh/)

  TLDR is a man-like package that serves as a tldr page for various commands and packages, instead of an in-depth manual (like man). A friend told me about this and I found this handy while trying to understand new linux commands. 

3. [Intro to Linux filesystems](https://opensource.com/life/16/10/introduction-linux-filesystems)

  The page above is a good read to prepare for Week 03 assignments. It helps to really understand what you're doing instead of copy-pasting commands.

## Week 04: Virtual Memory & C Pointers

1. [Virtual Memory: A Playlist](https://youtube.com/playlist?list=PLiwt1iVUib9s2Uo5BeYmwkDFUh70fJPxX)

  The playlist above provides excellent explanations into certain areas about Virtual Memory. I specifically found the video on Page Tables helpful.

2. [Pointers in C](https://youtu.be/mw1qsMieK5c)

  This week we delve deeper into C, with a highlight on pointers. My Week 02 links have been a good place to start, but the video above explains it in more detail.

## Week 05: Diving into Memory

1. [Understanding Page Faults](https://www.site24x7.com/learn/linux/page-faults-memory-swapping.html)

  This article explains the concept of page faults very well, even goes through memory swapping and more.

2. [Basics of Virtual Memory](https://youtu.be/8yO2FBBfaB0)

  This video from MIT OCW is a good starter to understand the idea of paging.

3. [Virtual Address Space](https://www.techtarget.com/searchstorage/definition/address-space)

  This article from Techtarget explains about Virtual vs Physical memory, as well as what address space is. The page also demonstrates how interconnected W04 and W05 are.

## Week 06: Kernel & Processes

1. [Upgrading Linux Kernel](https://linuxhint.com/upgrade-linux-kernel-version-debian-10/)

  This guide on upgrading your kernel is comprehensive and useful to refer back if ever needed again.

2. [pstree manual](https://man7.org/linux/man-pages/man1/pstree.1.html)

  While pstree is not installed by default, this command is a useful tool to help visualize processes and their child threads.

3. [How to Clean a Linux Zombie](https://www.baeldung.com/linux/clean-zombie-process)

  One of the main points of interest this week were zombie & orphan processes. The page above helps to get a better understanding of zombies in particular.

## Week 07: Synchronization

1. [Critical Section Animation](https://youtu.be/6x_XMDCMyAk)

  The critical section problem is an issue where there is a resource that can only be used by one process at a time, but multiple processes want to use it. That concept is visualized with an analogy by the video above, which helps to understand the criteria/conditions for solving this problem.

2. [Operating Systems: Process Synchronization](https://www.cs.uic.edu/~jbell/CourseNotes/OperatingSystems/5_Synchronization.html)

  The page above is an excellent summary (though still very long and detailed) of the entire chapter of Synchronization, from its concept to different solutions like Peterson's Solution (software-based) and Semaphores (hardware solution). The page also includes snippets of C code to help us understand the problems and solutions in practice.

3. [What is a semaphore?](https://youtu.be/ukM_zzrIeXs)

  Aside from mutual exclusion (mutex), another approach that you can take in solving the critical section problem is using semaphores. The video above is quite informative and well-explained.

## Week 08: Scheduling & Linux From Scratch

1. [CPU Thread Scheduling PCS SCS](https://youtu.be/hnP2f51flGg)

  This is a brief video that some concepts of thread scheduling such as the difference between user-level threads and kernel-level threads. The video explains that user-level threads are mapped to kernel-level threads, and also differentiates Process Contention Scope (PCS) with System Contention Scope (SCS). This video also uses the reference textbook OSC10.

2. [Multi-processor Scheduling](https://www.scaler.com/topics/operating-system/multi-processor-scheduling/)

  This article by Scaler elaborates how scheduling works in multiple processor systems and multi-core processors. They summarize concepts from this chapter very concisely.

3. [Memahami BUG: soft lockup](https://nicolas.my.id/memahami-apa-itu-BUG-soft-lockup-CPU-X-stuck-for-XXs/)

  This clean and useful article by Nicolas Julian explains a problem that some people and I encountered while building Linux from Scratch. The solution and explanation offered actually worked and allowed me to continue compiling packages without my debian host hanging :')

4. [What is a Linux Swap Partition](https://www.makeuseof.com/tag/swap-partition/)

  During the building of Linux from Scratch, I had to dig deeper into what the swap partition of /var/tmp.swapfile.bin was for, and what it actually did. Tip: Don't be like me, read Chapter 2.7 carefully and make sure you append the swap partition to /etc/fstab. 
