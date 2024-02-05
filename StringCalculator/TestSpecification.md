# StringCalculator

## Scenarios

### 1. Empty String Input

**Given** an empty string `input = ""`  
**When** `add()` is called  
**Then** the result should be `0`

---

### 2. Single String Input

**Given** a single string `input = "1"`  
**When** `add()` is called  
**Then** the result should be `1`

---

### 3. Two Numbers Separated by Delimiter

**Given** two numbers separated by a delimiter, `input = "1,2"`  
**When** `add()` is called  
**Then** the result should be `3`

---

### 4. Negative Value in String Input

**Given** a negative number in the string input, `input = "-1,2"`  
**When** `add()` is called  
**Then** an exception should be thrown with the message `"negatives not allowed"`

---

### 5. Newline Separator Between Numbers

**Given** numbers separated by a newline, `input = "1\n2,3"`  
**When** `add()` is called  
**Then** the result should be `6`

---

### 6. Number Above 1000

**Given** a number above 1000, `input = "2,1001"`  
**When** `add()` is called  
**Then** the result should be `2`

---

### 7. Support Different Delimiter

**Given** a different delimiter, `input = "//;\n1;2"`  
**When** `add()` is called  
**Then** the result should be `3`

---

### 8. Support Any Length of Delimiter

**Given** any length of delimiter, `input = "//[***]\n1***2***3"`  
**When** `add()` is called  
**Then** the result should be `6`

---

### 9. Support Multiple Delimiters

**Given** multiple delimiters, `input = "//[*][%]\n1*2%3"`  
**When** `add()` is called  
**Then** the result should be `6`
