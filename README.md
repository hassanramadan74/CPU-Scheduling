# CPU-Scheduling

CPU scheduling algorithms are an essential part of an operating system's task management. They determine the order in which processes are executed on a computer's CPU. Here's a summary of some popular CPU scheduling algorithms:

First-Come, First-Served (FCFS):
Processes are executed in the order they arrive.
Non-preemptive: Once a process starts executing, it continues until it completes or blocks.
Simple implementation but suffers from poor average waiting time, especially if long processes arrive first (the "convoy effect").

--------------------------------------------------------------------------------------------------------------------------------------------------------
Shortest Job Next (SJN) or Shortest Job First (SJF):
Selects the process with the shortest burst time to execute next.
Non-preemptive: Once a process starts executing, it continues until it completes or blocks.
Minimizes average waiting time and provides optimal results but requires knowledge of burst times in advance (which is often impractical).

--------------------------------------------------------------------------------------------------------------------------------------------------------
Priority Scheduling:
Each process is assigned a priority, and the process with the highest priority executes first.
Non-preemptive: Once a process starts executing, it continues until it completes or blocks.
Can suffer from starvation (low-priority processes waiting indefinitely) if not properly implemented.

--------------------------------------------------------------------------------------------------------------------------------------------------------
Round Robin (RR):
Processes are executed in a cyclic manner, each given a fixed time quantum or time slice.
Preemptive: Processes are interrupted after their time quantum expires and moved to the back of the queue.
Provides fair execution and responsiveness, but can lead to high context switching overhead if the time quantum is too small.
