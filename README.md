# PDF Renamer for PDF Documents
## Overview

The renamePDF_map.py script is designed to automate the process of renaming PDF files based on names extracted from their content, specifically looking for names followed by ", Kindergarten". The script matches these names against an Excel file that contains corresponding IDs, and renames the PDFs to these IDs, ensuring unique filenames in the target directory.

## Features

- Extract names from PDF files using text extraction.
- Match names with IDs in a specified Excel sheet.
- Rename PDFs with unique filenames based on their IDs.
- User-friendly interface for selecting files and directories.

## Dependencies

Python 3.x
pdfplumber
pandas
tkinter

## Installation

### Prerequisites

Ensure you have Python installed on your system. You can download Python from python.org.

### Required Libraries

Install the required Python libraries using pip:

    pip install pandas pdfplumber

*Note:* tkinter typically comes pre-installed with Python. You may need to install it via your system's package manager if it's not installed.

## Usage

**1- Start the Script:**

  + Navigate to the script's directory in your terminal or command prompt.
  + Run the script using Python:
  
      python renamePDF_map.py

    
**2- Select the PDF Directory:**
  
  A file dialog will open. Select the directory that contains the PDF files you want to rename.

**3- Select the Excel File:**
  
  Another file dialog will open. Select the Excel file that contains the name-ID mappings.

**4- Choose the Excel Sheet:**

  A simple dialog will prompt you to enter the name of the Excel sheet that contains the necessary data.

**5- Automatic Renaming:**

  The script will process each PDF file in the selected directory, extract names, find corresponding IDs, and rename the files accordingly.

## Troubleshooting

+ **ModuleNotFoundError:** Make sure all dependencies are installed. Re-run the installation commands if necessary.
+ **No names found:** Check the PDF files to ensure they contain selectable text and not images of text.
+ **Excel file issues:** Ensure the Excel file is correctly formatted with columns named 'Name' and 'ID'.

## Contributing
Feel free to fork this repository and submit pull requests. You can also send me patches or email me with any other improvements you think of.

## License
This script is provided "as is", without warranty of any kind. You can use and modify it as you need.

