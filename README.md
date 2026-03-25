Job Sequencing with Deadlines (C++)
📖 Overview
This project implements the Job Sequencing with Deadlines problem using a greedy algorithm in C++.
The goal is to maximize total profit by scheduling jobs within their deadlines. Each job takes 1 unit of time, and only one job can be scheduled at a time.
🚀 Features
Sorts jobs based on maximum profit
Efficiently schedules jobs within deadlines
Calculates:
Total number of jobs completed
Maximum profit earned
Optimal job sequence
🧠 Algorithm Used
Greedy Approach
Sort all jobs in descending order of profit
Find the maximum deadline
Create a time slot array
Assign each job to the latest available slot before its deadline
Compute total profit and job count
📂 Code Structure
🔹 struct Job
Represents a job with:
id → Job ID
deadline → Last time slot to complete job
profit → Profit earned
🔹 compare()
Custom comparator to sort jobs by profit (descending).
🔹 jobSequencing()
Main function that:
Sorts jobs
Allocates time slots
Assigns jobs optimally
Prints results
🔹 main()
Initializes job list
Calls the sequencing function
🧾 Example Input
Job arr[] = {
    {1, 2, 100},
    {2, 1, 19},
    {3, 2, 27},
    {4, 1, 25},
    {5, 3, 15}
};
📊 Example Output
Number of jobs done: 3
Total profit: 142
Job sequence: J1 J3 J5
⚙️ How to Run
🖥️ Compile
g++ job_sequencing.cpp -o job
▶️ Execute
./job
⏱️ Time & Space Complexity
Type	Complexity
Time	O(n²)
Space	O(n)
📌 Applications
Task scheduling
CPU job scheduling
Project management optimization
Resource allocation problems
