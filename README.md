# Module 5 - Java Profiling

## Reflection
### Performance Testing with JMeter vs Profiling with IntelliJ Profiler
The difference between the approach of performance testing with JMeter and profiling with IntelliJ Profiler in the context of optimizing application performance is:
JMeter is used to measure the performance of an application by simulating high workload on the application (the application is used by many people simultaneously with simulator group), while IntelliJ Profiler is used to identify bottlenecks in the application that cause slow application performance. 
### How Does Profiling Help Me Identify and Understand The Weak Points in My Application?
Profiling helps me identify the bottleneck in my application. It analyzes which points in my application that reduce its performance and offering insights by giving CPU usage, memory allocation, and thread concurrency.
### Is IntelliJ Profiler Effective?
I do believe that it is effective because it provides me insights by visualizing which part in my application that takes too much time to execute. Moreover, it also gives me visualization of execution time, so that I can easily know which part of my app that needs to be enhanced.
### The Main Challenges When Conducting Performance Testing & Profiling
For me, the main challenges when conducting performance testing and profiling are understanding how to read the data that IntelliJ and JMeter provided & how to optimize my application after knowing which part that I should optimize.
### The Main Benefits I Gained from Using IntelliJ Profiler for Profiling
The main benefit that I gained from using IntelliJ Profiler for profiling is that it is easy to use. Moreover, I have no need to use other softwares or third-party applications to conduct profiling.
### How Did I Handle Inconsistent Situations from Both Approaches?
When both approaches give different (and inconsistent) results, I consider the chances on why it might occur. For instance, the distinct functionalities of both approaches. However, if it still occurs even though I have tried to fix the inconsistency multiple times, I might ask for help from the teaching assistants and lecturers.
### Strategies That I Implemented in Optimizing My Application Code After Analysis
1. Optimizing data structure for memory allocations: I implement this when I utilize StringBuilder instead of String concatenation (joinStudentNames)
2. Optimizing query: I implement this when I just go for searching the highest rank by GPA for students instead of iterating them one by one. (findHighestGPA)
3. Optimizing number of database calls: I implement this when I utilize Hashmap instead of List for accessing 'daftar siswa' (getAllStudentsWithCourses)
## JMeter Report and Test Results
### *Endpoint* `/all-student`
Test Result from JMeter:
<img src="src/image/all-student-request (result).png" alt="all-student-request">
Before Optimization:
<img src="src/image/all-student-request (before).png" alt="all-student-request">
After Optimization
<img src="src/image/all-student-request (after).png" alt="all-student-request">
### *Endpoint* `/all-student-name`
Test Result from JMeter:
<img src="src/image/all-student-name (result).png" alt="all-student-name">
Before Optimization:
<img src="src/image/all-student-name (before).png" alt="all-student-name">
After Optimization
<img src="src/image/all-student-name (after).png" alt="all-student-name">
### *Endpoint* `/highest-gpa`
Test Result from JMeter:
<img src="src/image/highest-gpa (result).png" alt="highest-gpa">
Before Optimization:
<img src="src/image/highest-gpa (before).png" alt="highest-gpa">
After Optimization
<img src="src/image/highest-gpa (after).png" alt="highest-gpa">
