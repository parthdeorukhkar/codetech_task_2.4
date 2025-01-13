# codetech_task_2.4

SMS Spam Collection Data Extraction and Loading
This Python script automates the process of extracting and loading the SMS Spam Collection dataset. The dataset contains labeled SMS messages for binary classification as "spam" or "ham" (not spam).

Features
Extract Dataset:

Extracts the SMS Spam Collection dataset from a ZIP file.
Lists the extracted files.
Load Data:

Reads the dataset into a Pandas DataFrame.
Assigns column names label and message for better readability.
Preview Dataset:

Displays the first few rows of the dataset for verification.
Requirements
Install Required Libraries:
pandas: For data loading and manipulation.
zipfile: To extract the ZIP archive.
os: For file system interactions.
Install the required Python packages:

bash
Copy code
pip install pandas
Setup and Usage
1. Download the Dataset
The dataset ZIP file can be downloaded from the UCI Machine Learning Repository:

SMSSpamCollection.zip
Place the ZIP file (smsspamcollection.zip) in the script's working directory.

2. Run the Script
Execute the script using:

bash
Copy code
python script_name.py
Replace script_name.py with the name of your script.

3. Output
The script:

Extracts the ZIP file into a folder named smsspamcollection.
Prints the list of extracted files.
Loads the SMSSpamCollection dataset into a DataFrame.
Displays a preview of the first five rows.
Example Output
Extracted Files
less
Copy code
Extracted files: ['SMSSpamCollection', 'readme']
Dataset Preview
css
Copy code
     label                                            message
0      ham  Go until jurong point, crazy.. Available only ...
1      ham                      Ok lar... Joking wif u oni...
2     spam  Free entry in 2 a wkly comp to win FA Cup fina...
3      ham  U dun say so early hor... U c already then say...
4      ham  Nah I don't think he goes to usf, he lives aro...
Dataset Details
The SMSSpamCollection dataset contains two columns:

label:
ham: Non-spam messages.
spam: Spam messages.
message:
The content of the SMS message.
Statistics
Total samples: 5574.
Spam samples: ~13.4%.
Ham samples: ~86.6%.
Error Handling
1. Missing ZIP File
If the ZIP file (smsspamcollection.zip) is not present in the working directory, the script will fail. Ensure the file is downloaded manually from the UCI repository.

2. Missing or Corrupted Files
If the ZIP file does not contain the expected dataset, verify the source file's integrity.

Future Enhancements
Automate dataset downloading using requests.
Add visualizations for label distribution (e.g., pie chart or bar graph).
Provide options for basic text preprocessing (e.g., tokenization, stop-word removal).

![WhatsApp Image 2025-01-13 at 20 37 06_3b31e21b](https://github.com/user-attachments/assets/5b9e792b-c223-4ddb-9226-736d1f447029)
