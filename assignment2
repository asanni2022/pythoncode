## Python GitHub Action
### Log Analyzer:
Scenario: As an IT administrator, you often have to sift through logs to find errors. Write a Python program that analyzes a log file and reports any errors found.

Question: Create a function called find_errors that reads through a file named 'system.log'. Every line that starts with the word "ERROR" should be captured and written to a new file called 'error.log'. After processing the file, the function should also print out the total number of errors detected.

Hint:

Use the startswith() string method to check if a line begins with "ERROR".
Employ file handling operations to read from 'system.log' and write to 'error.log'.

'''
def find_errors():
    # Open the input log file for reading and the output error file for writing
    with open('system.log', 'r') as input_file, open('error.log', 'w') as output_file:
        error_count = 0  # Counter to keep track of the number of errors
        
        for line in input_file:
            if line.startswith("ERROR"):
                # Write the error line to the error.log file
                output_file.write(line)
                error_count += 1
        
        # Print the total number of errors detected
        print(f"Total number of errors detected: {error_count}")

# Call the function to start the log analysis
find_errors()

'''
