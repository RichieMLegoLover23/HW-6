# HW-6
#1

# Open the file for writing
with open("things.txt", "w") as f:
    # Write the name of an animal to the file
    f.write("lion\n")
    
    # Write the name of a fruit to the file
    f.write("apple\n")
    
    # Write the name of a country to the file
    f.write("Japan\n")
    
# Close the file (this happens automatically when the "with" block ends)



























#2
# Open the file for reading
with open("things.txt", "r") as f:
    # Read all the data from the file
    data = f.read()
    
# Display the data
print("Data from file:")
print(data)





























#3
# Open the file for writing
with open("number_list.txt", "w") as f:
    # Loop from 1 to 100
    for i in range(1, 101):
        # Write the number to the file
        f.write(str(i) + "\n")
        
# Close the file (this happens automatically when the "with" block ends)





























#4
# Open the file for reading
with open("numbers.txt", "r") as f:
    # Read all the lines from the file and convert them to integers
    numbers = [int(line.strip()) for line in f.readlines()]

# Calculate the total of the numbers
total = sum(numbers)

# Display the total
print("Total of the numbers in the file:", total)
