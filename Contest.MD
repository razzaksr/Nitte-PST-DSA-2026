Day1 Assignments:
1. https://leetcode.com/problems/remove-duplicates-from-sorted-array/description/
2. https://leetcode.com/problems/third-maximum-number/description/
3. https://leetcode.com/problems/find-pivot-index/description/

Day2 Assignments:
1. https://leetcode.com/problems/set-matrix-zeroes/
2. https://leetcode.com/problems/valid-palindrome/

Day3 Assignments:
1. https://leetcode.com/problems/power-of-three/description/
2. https://leetcode.com/problems/reverse-bits/description/
3. https://leetcode.com/problems/single-number/description/

Day4 Assignments:
1. https://leetcode.com/problems/search-insert-position/description/
2. https://leetcode.com/problems/fair-candy-swap/description
3. Problem Statement: Loan Application Management System
Context:  
A small financial institution wants to build a simple Java application to manage loan applications. Each applicant can apply for multiple loans, view their current loans, and cancel them if needed. The system should be modular, using abstract classes and overriding to enforce a contract while allowing flexibility in implementation.

Requirements:
Create an abstract class LoanRemote that declares the following abstract methods:
applyLoan(int applicantId, String loanType)
viewLoan(int applicantId)
cancelLoan(int applicantId)

Additionally, include a concrete helper method log(String message) to print system logs.
Implement a concrete subclass LoanService that overrides all abstract methods.
Use a 2D array (String[][] loans) to store loan applications.
Rows represent applicants.
Columns represent loan slots for each applicant.
applyLoan should add a loan type to the applicant’s record if space is available.

viewLoan should display all loans for a given applicant.
cancelLoan should clear all loans for a given applicant.
Create a driver class LoanDemo with a main method to test the functionality.
Apply multiple loans for different applicants.
View loans before and after cancellation.
Demonstrate system logs printed by the helper method.

Expected Output (Sample Run):
Loan applied: Personal Loan for applicant 0
Loan applied: Business Loan for applicant 0
Loan applied: Education Loan for applicant 1
Applicant 0 loans: [Personal Loan, Business Loan]
Loans cancelled for applicant 0
Applicant 0 loans: [null, null]


Day5 Assignments:
1. Problem Statement: Meeting Rooms
You are given an array of meeting time intervals, where each interval is represented as [start, end]. A person can only attend one meeting at a time.
Write a function canAttendMeetings(int[][] intervals) that determines if a person can attend all meetings without any overlaps.

Example 1
Input:
intervals = [[0,30],[5,10],[15,20]]
Output:
false
Explanation:  
Meeting [0,30] overlaps with [5,10] and [15,20]. The person cannot attend all meetings.

Example 2
Input:
intervals = [[7,10],[2,4]]
Output:
true
Explanation:  
No meetings overlap. The person can attend all meetings.

Constraints
0 <= intervals.length <= 10^4
intervals[i].length == 2
0 <= start < end <= 10^6

2. https://leetcode.com/problems/house-robber/description/
3. Validate IPv4 using regex, custom exception and logs

Day6 Assignments:
1. https://leetcode.com/problems/valid-parentheses/
2. https://leetcode.com/problems/daily-temperatures/description/

Day7 Assignments:
1. https://leetcode.com/problems/majority-element/
2. https://leetcode.com/problems/word-pattern/description/

Day8 Assignments:
1. Serialized POJO Class: Feedback contains properties of trainerName(String), batchId(String), studentUsn(String), rating(double), comments(String)
    perform followings:
    1. store atleast 3 feedbacks objects as list into file
    2. read feedbacks by usn


Day9 Assignments:
1. https://leetcode.com/problems/building-h2o/description/
2. https://leetcode.com/problems/squares-of-a-sorted-array/


Day10 Assignments:
1. https://www.hackerrank.com/challenges/array-left-rotation/problem
2. Create the following tables and generate ER Diagram:
    Customer(CustomerID, CustomerName, DOB, ContactNo)
    PolicyType(PolicyType, PremiumRate, CoverageYears)
    Branch(BranchID, BranchName, Manager)
    Policy(PolicyID, CustomerID, PolicyType, PremiumAmount, BranchID)

    Insert sample data:
    Customers:
    C1: Ramesh, 1985‑05‑10, 9876543210
    C2: Kavya, 1990‑09‑15, 9123456789

    PolicyTypes:
    Health – 5% premium, 10 years coverage
    Life – 8% premium, 20 years coverage
    Vehicle – 6% premium, 5 years coverage

    Branches:
    B1: Bangalore – Manager: Anil
    B2: Mysore – Manager: Sneha

    Policies:
    P1: Ramesh, Health, 20000, Bangalore
    P2: Ramesh, Vehicle, 15000, Bangalore
    P3: Kavya, Life, 50000, Mysore


Day11 Assignments:
1. Create the following tables and perform following aggregations:
    Customer(CustomerID, CustomerName, DOB, ContactNo)
    PolicyType(PolicyType, PremiumRate, CoverageYears)
    Branch(BranchID, BranchName, Manager)
    Policy(PolicyID, CustomerID, PolicyType, PremiumAmount, BranchID)

    Insert sample data:
    Customers:
        C1: Ramesh, 1985‑05‑10, 9876543210
        C2: Kavya, 1990‑09‑15, 9123456789

    PolicyTypes:
        Health – 5% premium, 10 years coverage
        Life – 8% premium, 20 years coverage
        Vehicle – 6% premium, 5 years coverage

    Branches:
        B1: Bangalore – Manager: Anil
        B2: Mysore – Manager: Sneha

    Policies:
        P1: C1, Health, 20000, B1
        P2: C1, Vehicle, 15000, B1
        P3: C2, Life, 50000, B2

    a. Write a query to find the maximum premium amount per branch.
    b. Write a query to list customers who have more than one policy.
    c. Write a query to calculate the total annual premium payable per branch.


2. Consider the above tables and perform below DCL:
    a. Log in as branch_manager and try to:
        Insert a new policy → should succeed.
        Update an existing policy → should fail after revoke.

    b. Log in as policy_auditor and try to:
        Run SELECT * FROM Policy; → should succeed.
        Run INSERT INTO Policy ... → should fail.

    c. Log in as policy_admin and try to:
        Drop a table → should succeed.
        Grant privileges to another user → should succeed.