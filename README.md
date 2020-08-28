# AI-Champ-Marathon-Tasks <br>
The code for all the tasks is stored in **Submition.ipynb** notebook. <br>

## Task 1 <br>
The LinkedIn profiles of 50 random people are downloaded and stored in the folder named: **PDF Files**

## Task 2 <br>
The **textract** library is used to extract the text from the downloaded PDFs. <br>
The ***extract_to_csv*** function takes the path of the folder containing the PDFs, extracts the text from it (using **textract** library) and stores the text in .csv file named ***CSV_file.csv***. <br>
The text extracted from the each PDF is added as a new row in the ***CSV_file.csv***.

## Task 3 <br>
The raw data extracted from the PDF, contains many **Stop words** (ex: 'i', 'me', 'here', 'there', 'when' etc), **Punctuation marks / Symbols** (ex: !"#$%&'()) and **Numbers** that are not usefull to find the most frequent words. Thus I have removed them from the word corpus. <br>
The ***preprocess_text*** function takes the text data extracted from PDF; removes Stop words, Punctuation marks / Symbols, Numbers from it and convert the remaining words to lowercase. <br>
This function is used on all PDFs and the cleaned corpus obtained is stored in ***words_list***. <br>
The ***get_frequency*** function takes a list containing words and gives the frequency of each word as a dictonary in format *{word: frequency}*. <br> 
The frequencies for all words are stored in ***frequency.***  <br>
The ***heapq*** library is used to get the top k most frequent words stored in  ***frequency***. <br>

## Task 4 <br>
I do not have any experience in web app development. Thus I could not finish the the 4th task.
