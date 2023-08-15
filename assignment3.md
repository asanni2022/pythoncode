## Python GitHub Action
### Log Analyzer:
Scenario: As an IT administrator, you often have to sift through logs to find errors. Write a Python program that analyzes a log file and reports any errors found.

Question: Create a function called find_errors that reads through a file named 'system.log'. Every line that starts with the word "ERROR" should be captured and written to a new file called 'error.log'. After processing the file, the function should also print out the total number of errors detected.

Hint:

Use the startswith() string method to check if a line begins with "ERROR".
Employ file handling operations to read from 'system.log' and write to 'error.log'.

```
def find_errors():
    input_file_path = 'system.log'
    output_file_path = 'error.log'
    
    total_errors = 0
    
    with open(input_file_path, 'r') as input_file, open(output_file_path, 'w') as output_file:
        for line in input_file:
            if line.startswith("ERROR"):
                output_file.write(line)
                total_errors += 1
    
    print(f"Total errors detected: {total_errors}")

# Call the function to start processing
find_errors()

```
