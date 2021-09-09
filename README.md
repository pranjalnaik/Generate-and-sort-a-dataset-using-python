# Homework0-DataIntensiveComputing
Authors - Pranjal Naik , Shrey Kothari , Dhaval Patel

Directory Structure -
            *generate-dataset.sh
            *sort-data.sh

#Run the command in screen so that the execution of script isnt stopped because of issues in ssh
            screen generatedata

#Run the below command for generating a data set with first column of 32-bit integer and second column of 95 bytes of ASCII string.
#It will also provide the time taken by the system in generating the dataset.
#2>/dev/null will take care of the errors and warnings
            time ./generate-dataset.sh yellow 10000 2>/dev/null
#A file called "yellow" will be generated with 10000 rows

#Run the below command to sort the data using the first column using bash script
#2>/dev/null will take care of the errors and warnings
            time ./sort-data.sh 2>/dev/null
#A file called "sorted_yellow" will be generated with 10000 rows

#Run the below command to sort the data using the first column using C program
            gcc sort.c -o gcc
            ./gccy

#Run the below command to sort the data using the first column using Python program
            python3 sort.py
#This will create a file "sorted_yellowPython" with 10000 rows




