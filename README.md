# Data Hunters - Web Scraping Project
This project involves web scraping to identify and extract specific CSV files from GitHub repositories. The target CSV files need to meet certain submission criteria, and this project will handle various scenarios to ensure the correct files are identified and processed.

## Project Description
This project was developed to automate the process of finding CSV files that meet specific submission criteria from a list of GitHub repositories. The program addresses several scenarios to ensure accurate and efficient data extraction.

**Scenarios Covered:**
1. **Case1:** if there are many such files, ur code should be able to capture the most recent uploaded file. 
2. **Case2:** if there is no such file, ur code should report that. 
3. **Case3:** say you found a csv file, but it fails to suffice the submission criterion, ur code should ignore that and move to the next, until you land at Case1/Case2. 
4. **Case4:** The provided link isnt even of github, again ur code should report it. 
5. **Case5:** The csv file may be in some folder, more may be in folder of folders, ur code should be able to deal with that too, to land at case1/case2. 

## Project Files

- `chromedriver.exe`: The ChromeDriver executable required for web scraping.
- `links_of_submission.xlsx`: The input file containing GitHub repository links.
- `mains.py`: The main script that performs the web scraping and data processing.
- `output.txt`: The output file containing the results of the script execution.
- `submission_format.csv`: The file used to define the submission criteria(submitted file should not be exactly same as this).

## Prerequisites
Before you begin, ensure you have met the following requirements:
- Python
- pip (Python package installer)
- Google Chrome browser
- **Download and install ChromeDriver:**
    - [ChromeDriver Download](https://sites.google.com/a/chromium.org/chromedriver/downloads)
    - Ensure the downloaded `chromedriver.exe` is placed in the project directory.

## Setup Instructions

1. **Clone the repository:**
    ```bash
    git clone https://github.com/musk1n/Data-Hunters.git
    cd Data-Hunters
    ```

2. **Create a virtual environment and activate it:**
    ```bash
    python -m venv venv
    source venv/bin/activate   # On Windows, use `venv\Scripts\activate`
    ```

3. **Install the required packages:**
    ```bash
    pip install -r requirements.txt
    ```
## Running the Project
1. **Execute the main script:**
    ```bash
    python mains.py
    ```
You will notice the output same as in output.txt file

## Credits
- Subhashree Kedia - https://github.com/SKed72274
- Muskan - https://github.com/musk1n
