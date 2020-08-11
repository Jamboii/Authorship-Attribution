CSC470 Natural Language Processing - Project 4 Report
Authorship Attribution
Alex Benasutti, Samuel Bishop, and Chris Jenson

Task: In this project you will gain hands-on experience working in a team to implement  authorship  attribution  systems  from  scratch.   You  will  also  gain additional hands-on practice applying and continuing to increase your foun-dational corpus processing and language modeling skills.  You will also gain experience  in  production  of  professional  well  documented  software  deliver-ables and reports.

README File

From a Mac in STEM112:


Creating the training and test datasets (T1-T2):
1. Open the terminal
2. Navigate to the location where the “Project4.tar.gz” file was downloaded
3. Ex. if downloaded to Downloads, enter “cd Downloads”
4. To extract the “Project4.tar.gz” file, type "tar -zxvf Project4.tar.gz"
5. Type “Project4” to enter the extracted folder named Project4 containing the Python code
6. Type “python3 t2.py path1 path2 path3”, and hit enter. Path1 is the path to the 7. imdb62.txt file, path2 is the path to where the train directory will be created, and path3 is the path to where the test directory will be created
   6.1. The paths should not already contain directories named “train” or “test”
7. The program will then output to those directories

Example: $ t2.py /path/to/imdb62.txt /path/to/train /path/to/test 

NOTE: The $ sign is just a symbol to represent a linux-style command-line prompt.  The user wouldn’t actually type the $ sign.

NOTE: If the specified directories already exist, the program will say that the creation of them failed.


Running the authorship attribution systems (T3-T5):
1. Inside the project directory, and having created both training and test sets, type the following command in the terminal:
   1.1. python3 t4.py path1 path2 path3
   path1: Training data directory (ex. ./train/) 
   path2: Test data directory (ex. ./test/)
   path3: Author data text file (ex. ./authors.txt)
2. The authorship attribution systems for AllTokens and Singletons will be run using the training and test data on the authors supplied in path3.
3. A ranked list for each system will be displayed to the terminal, and outputted to a text file. Each element of the ranked list is labeled as such: (AuthorID, systemScore)


Individual File Description:

README.txt -> This README file.

authors.txt -> List of authors to be input into the author attribution system.

/train/ -> Randomly sampled idmb62 training directory (from t2.py).

/test/ -> Randomly sampled imdb62 test directory (from t2.py).

t2.py -> Python source file containing code for T2.

t3.py -> Python source file containing code for T3.

t4.py -> Python source file containing code for T4 and T5 that uses the base established in t3.py and runs the experiments in T5.

D3.txt -> Analysis as described in T5.

report.txt -> Responses to the questions as described in D4.
