Aim:
To compare file-copying performance using different buffer sizes and evaluate the number of read() system calls.

Observation:
TDifference Between Buffered I/O and Memory Mapping (mmap)
Working Method
Buffered I/O: Uses read() and write() system calls.
Memory Mapping (mmap): Maps file contents into virtual memory.
Data Access
Buffered I/O: Data is copied through a user-space buffer.
Memory Mapping: File contents can be accessed through memory addresses.
Implementation
Buffered I/O: Easy to implement.
Memory Mapping: Requires memory mapping and synchronization management.
Usage
Buffered I/O: Suitable for simple file-copying operations.
Memory Mapping: Useful for accessing and processing large files.
Comparison
Buffered I/O is simple and suitable for normal file-copying operations.
mmap() can reduce explicit read calls but still involves page faults and memory-management overhead.
Comparison:
•	Buffered I/O is simple and suitable for normal file-copying operations.
•	mmap() can reduce explicit read calls but still involves page faults and memory-management overhead.
•	The best method depends on file size and workload.
 Conclusion
Thus, file copying was successfully performed using different buffer sizes. The experiment demonstrates that increasing the buffer size reduces the number of read() system calls and improves file I/O efficiency. Among the tested buffer sizes, 4096 bytes required the fewest read calls.




