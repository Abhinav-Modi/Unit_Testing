1.Scenario: Empty string input
	Given = ""
	When  Add called
	Then return 0


2. Scenario: Single string input
	Given = "1"
	When Add called 
	Then return 1

3.Scenario: 2 numbers seperated by delimiter
	Given "1,2"
	When Add called
	Then return 3

4.Scenario: Negative value in string input
	Given "-1,2"
	When Add called
	Then return Exception(“negatives not allowed”)

5.Scenario: Newline separator between numbers
	Given "1\n2,3"
	When Add Called
	Then return 6

6. Scenario: When the number is above 1000
	Given "2,1001"
	When Add Called
	Then return 2

7. Scenario: Support Different delimiter
	Given "//;\n1;2"
	When Add Called
	Then return 3
8.Scenario: Support any length of delimiter
	Given "//[***]\n1***2***3"
	When Add Called
	Then return 6
9. Scenario: Support multiple delimiter
	Given "//[*][%]\n1*2%3"
	When Add Called
	Then return 6
