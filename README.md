# Baby Name Analysis Program

## Introduction

Good afternoon, my name is [Your Name], and we are Team Cobra. We are very excited to showcase our baby name analysis program along with the development process that we underwent to develop the final product.

Our team members:
- Adil Siddiqi - File processing and formatting
- Ben Holbrook - Testing and validation
- Megan D’costa - Question functions and analysis
- Yousuf Mohiuddian - Main file and UI development

## Project Overview

Our baby name analysis program processes, tests, and analyzes baby name data from various regions and provides insights through a series of functions. These insights can be visualized using graphs to better understand trends and patterns in baby names.

## Files and Structure

### Raw Data Files

All raw data files are provided in the `Raw_Data` folder. For each file, if there is a header or anything above the CSV data, those rows should be deleted before processing.

### Processing Scripts

Each region has a dedicated processing script to format and clean the data. The processed files must be placed in the `region` folder.

- **Alberta:** `./albertaProcessing -i <fileName>`
- **Ireland:** `./irelandProcessing -m <maleFileName> -f <femaleFileName>`
  - Note: The last half of the Ireland file was deleted as it contained a ranking system not aligned with our intended ranking system.
- **California:** `./california.py -i <input file name> -f <female output file name base> -m <male output file name base>`
- **Quebec:**
  - Male file: `./quebecBoys.py -i <input file name> -o <output file name base>`
  - Female file: `./quebecGirls.py -i <input file name> -o <output file name base>`
- **Ontario:** `./ontarioScript.py -m <maleFileName> -f <femaleFileName>`
- **Nova Scotia:** `./novaScotiaScript.py -i <inputFileName>`
- **Australia:** `./australiaScript.py -i <inputFileName>`
- **New Brunswick:** `./NBRead.py -i <inputFileName>`
- **New Zealand:** `./NZRead.py -i <inputFileName>`

### Main Program

The main program is run using `./main.py`. It includes various sections and helper functions to answer questions about baby names.

## Functionality

Our software offers eight question options to help users gain a deeper understanding of baby names:

1. **Average Length of Baby Names:** Calculates the average length of baby names in a certain location and year.
2. **Most Common Starting Letters:** Finds the 5 most popular starting letters of baby names in a certain location and year.
3. **Common Names Over Time:** Plots the number of common names between boys and girls over time for a given location.
4. **Total Frequency of a Name:** Outputs the total frequency of a given name across different regions.
5. **Average Rank of a Name:** Finds the average rank of a given name in each region.
6. **Most Popular Names by Letter:** Finds the most popular baby name that starts with each letter of the alphabet for a given location and gender.
7. **Most Popular Names by Vowel:** Finds the most popular baby name that starts with each vowel for a given location and gender.
8. **Ethnic Origin of Names (Beta):** Uses the Namsor service to determine the ethnic origin of names.

### Testing

Our testing script ensures that the processed files are in the correct format and meet our standards. We test for:
- Entries without names
- Duplicate names in the same year
- Incorrect rankings
- Entries with a frequency of 0
- And more...

### Visualization

The program provides options to visualize the data using various graphs, such as pie charts and line graphs.

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/megdcosta/baby-names-comparative-study.git
