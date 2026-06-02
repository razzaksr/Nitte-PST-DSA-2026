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