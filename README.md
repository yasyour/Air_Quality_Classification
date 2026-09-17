# Air_Quality_Classification

A C++ program that reads air quality index (AQI) data from a file and classifies each reading into a category, from "Good" to "Severe".

## Overview
It can be difficult for non-experts to understand the meaning behind the Air Quality Index unless each number is tied to a specific category. This program reads AQI readings for a set of buildings from a data file and classifies each one, from "Good" to "Severe," with higher values indicating poorer air quality and greater health risks.

## How it works
AQI values are classified into six categories:

| AQI Range |   Category   |
|-----------|--------------|
|   0–50    |     Good     |
|   51–100  | Satisfactory |
|  101–200  |   Moderate   |
|  201–300  |     Poor     |
|  301–400  |   Very Poor  |
|  401–500  |    Severe    |


The program provides a menu with three options:
1. Conduct the air analysis: It reads AQI data from an input file, classifies each reading and saves the results to an output file. To conduct the analysis, make sure a file named `input.txt` containing your AQI data is present in the same directory, this is the fixed input file the program reads from. You'll then be prompted to enter a name for the output file.
2. Display results: It prints a previously generated output file to the screen (shows an error if Option 1 hasn't been run yet)
3. Exit the program

Each AQI value is checked for validity, so non-numeric entries are labeled "Corrupted data" so they don't affect classification.

## How to run
Compile and run the program, then follow the on screen menu.

## Example
| Building | AQI |    Category    |
|----------|-----|----------------|
|    D1    | **  | Corrupted data |
|    B2    | 49  | Good           |
|    C3    | 100 | Satisfactory   |
|    A1-C  | 194 | Moderate       |
|    A1-A  | !!  | Corrupted data |
|    C2    | 198 | Moderate       |

## Documentation
Full write up with test cases and algorithm design: [Air_Quality_Classification_Report.docx.pdf](https://github.com/user-attachments/files/32325581/Air_Quality_Classification_Report.docx.pdf)
