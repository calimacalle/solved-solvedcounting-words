Download Link: https://assignmentchef.com/product/solved-solvedcounting-words
<br>
Objectives The goal of this project is for you to master (or at least get practice on) the following tasks: • implementation of a reference based sorted list, • implementation of a reference based binary search tree with recursive methods.Problem Description Given an input text file compute a list of all unique words and count how many times they occur. Repeat this with linked list and binary search tree as the choice of the data structure for storing words to compare their relative performance. The program running time and word count information are written to the standard output (console). The user specified number of words together with their counts are written to the output file whose name should be provided on the command line.Input/Output The program is not interactive. The only input is provided on the command line. The program should expect three command line arguments: • the name of the input file, • an integer value indicating the cutoff value for the word counts that should be printed to the output file, • and the name of the output file. The program needs to validate all command line parameters. If they are missing or invalid, the program should print an error message and terminate. The input file is a text file that contains an arbitrary collection of words. The program should use the provided FileParser class to obtain a list of clean words from the input. Read the documentation for that class to learn how to use it. The program should catch and handle the exceptions that FileParser class throws. The output file should contain the list of the most frequently occurring words together with their counts. The second parameter on the command line specifies the cutoff value of the words that should be printed to the output file – only the words whose count is above or equal to the cutoff value should be printed to the output file. The structure of the output file should be as follows:Processing of data Populating the data structures Once your program uses FileParser to obtain the list of all the words from the input file, it should store them in two different data structures: 1) a sorted linked list, 2) a binary search tree. The nodes in the list/tree should store unique words (no repetitions allowed) together with their counts. As the program goes through the list of all words provided by the FileParses object it needs to decide if the next word already exists in the structures or not. If it does exist, the count for the corresponding word should be incremented. If it does not exist, a new entry should be created with count 1 and added to each structure. Computing the most frequent words In order to find the N most frequent words in the input file, your program needs to find the N words with the highest counts in both data structures. This task should be accomplished by pruning the list and the tree. Traverse each data structure and remove all nodes that contain words whose count is below the cutoff value. After pruning both structures should contain identical words. The words remaining in one of the structures should be then printed to the output file (do not print the content of both structures to the output file). Performance measurements The program should time how long it takes to 1) construct a structure given an ArrayList containing all the words from the input file, 2) prune the structure given the cutoff value. The program should display to the console all information regarding the timing and sizes of the structures at each stage. T