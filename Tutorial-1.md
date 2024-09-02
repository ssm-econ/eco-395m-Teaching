Bash exercise

1. Change working directory to your desktop
2. Make a folder called ECO395m
3. Make a folder called Tutorial 1 within it. 
4. Create a text file called intro.txt
5. Write your name and EID into that file using printf.
6. Using the echo command, add your email id into the file.
7. Use the grep command to find and extract the line with your email id (Use regular expressions here)





Learn about regular expressions here

Regular Expressions

Write regular expressions to match strings with the following patterns (be as specific as possible): 
Email addresses of the type <alphanumeric characters>@<alphanumeric characters>.com	\\
Phone numbers of the type : \\
Either (3 digits)-7 digits e.g (814)-3334563 OR
10 digits e.g 8143334563 [Should match both]
Website URLs: 
Either http://www.<alphanumerics>.com OR
www.<alphanumerics>.com [Should match both]
UT EIDs of the form <3 lowercase alphabet characters><4 digits> eg ssm3142
Strings beginning with the word “This” e.g “This is line number 1.”
Strings that end with a number of any length e.g “something something 45362”


Example solution: 1a: \w+@\w+.com













































Solution to Bash exercise

cd Desktop
mkdir ECO395m
mkdir Tutorial\	1
touch intro.txt
printf “My name is Shreeyesh. My EID is ssm3562.” >> intro.txt
echo “My email id is shreeyesh.menon@utexas.edu” > intro.txt
grep “\w+@\w+.com” intro.txt

Finally, to make an executable file with these commands, add #!/bin/bash at the top of the file

save it as introduction.sh and type the following command into the command line:
chmod u+x introduction.sh

You can then run the file by entering bash introduction.sh into the command-line.
 


