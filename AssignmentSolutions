CSE 340 Operating System Assignment 

By - Priyanshu Varshney (AU2340158) Group-11 

Answer 1:
It is sometimes difficult to create an operating system based on strictly layered approach when two components are tightly connected to each other. For example take the case of
CPU scheduling system and memory management system. For making efficient scheduling decisions, CPU scheduler often requires memory manager. For example, a process that is waiting for memory allocation may not be ready to run, and this information is necessary for the scheduler to know.
On the other hand, memory manager might also require CPU scheduler, to decide which process to keep in or remove from the memory. It must consider which processes are likely to run soon according to the scheduler's plan.
From this example, we can clearly realize that it is difficult to decide which layer should come above the other because both are dependent on each other's functionality. If we strictly put one onto the other, the design might become inefficient or complex. This is the reason why real-world operating system would rather use a more flexible approach than sticking to strict rules of layered design. 
Real Life Analogy: 
In a restaurent kitchen, where the chef (CPU scheduler) has to decide which dish to prepare first, but the ingredient manager (Memory manager) is responsible for the availability of ingredients. The chef cannot start cooking without ingredients and ingredient manager cannot decide what to bring without knowing chef's plan. They are tightly dependent on one another and we cannot place one above the other in a hierarchy. 

Answer 2:
The two main advantages of using microkernal approac are as follows:
1. Modularity 
2. Reliability 
In a microkernal, most important functions like communication between processes, low-level memory management, and basic scheduling run inside the kernal. Other functions like device drivers, networking, or file systems, run in user space as separate processes.
Interaction in microkernal architecture: User programs and system services interact through message passing. For example, if program wants to access a file, it sends a message to the file system service which is running in the user space. The file system service, handles the request and sends back the result. This approach ensures that even if one service goes down, the entire system does not crashes. 
Disadvantage of microkernal approach: The biggest disadvantage is performance overhead. Since services communicate with each other through message passing and not by direct function calls, there is a extra cost associated with context switching and copying data between user and kernal space. This makes microkernal systems slower than monolithic kernals. 
Real Life Analogy:
In a university, dean's office (the kernal) only handles most important duties like signing/approving official requests, while other departments like library,finance work independently and communicate with dean's office via written requests (messages). The advantage is that even if one department for example library fails, the entire university does not crumble. The disadvantage is that passing messages/requests back and forth is time consuming compared that everything is handled through a single office.

Answer 3:
Loadable kernal modules (LKMs) provide flexibility to operating system by allowing functionality to be added to the kernal at the runtime without needing to reboot the entire system. 
Advantages:
1. Flexibility:Features like device drivers, file systems, or network protocols can be loaded when required. This avoids keeping unnecesary code in the memory.
2. Efficiency: The kernal remains light-weight as modules can be loaded or unloaded dynamically, which results in better performance. 
3. Ease of maintenance: Developers can fix a module without modifying/reconstructing the entire kernal.
4. Customization: Different users can load only the modules they require which makes the operating system adaptable to different hardware or use cases. 
To summarize, LKMs make system more modular and easier to manage while reducing downtime. 
Real Life Analogy:
Imagine a brand new smartphone (kernal). It comes with pre-installed apps. If you need new functionality, you can download an app (module) without reinstalling the entire operating system. If you do not require the app anymore you uninstall it. In a simillar way, LKMs enables you to add or remove a features without disturbing the entire system.


