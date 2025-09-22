Student Information :

Name : Vishesh Vinshan Saraswat
Roll No. : 2401360027
University: K.R. Mangalam University
Course: Btech CSE (UX/UI)
Subject : Data Structure And Algorothms
Course Code: ENCS205 / ENCA 201


Weather Data Storage System 


A C++ command-line application designed to store, manage, and retrieve yearly weather data for multiple cities. This project was developed as part of the Data Structures (ENCS205/ENCA201) course at K.R. Mangalam University.
This has an capacity of supporting 8 major cities over a 15-year period (2011-2025).


Features :

Expanded Data Capacity: Pre-configured to handle data for 8 cities over 10 years.
Insert Record: Add a new temperature record for a specific city and year.
Delete Record: Remove an existing temperature record.
Retrieve Record: Look up and display the temperature for a specific city and year.
Display Data (Row-Major): View all stored records, iterated by Year, then City.
Display Data (Column-Major): View all stored records, iterated by City, then Year.
Sparse Data Handling: Uses NaN (Not a Number) as a sentinel value to manage city/year pairs with no recorded data.

Data Structure:

The core of the system is a 2D std::vector< std::vector <double>> that functions as a dynamic two-dimensional array. The dimensions are mapped as follows:
Rows ([year_index]): Each row corresponds to a year in the specified range.
Columns ([city_index]): Each column corresponds to a city from the predefined list.
This structure allows for direct O(1) access to the data for any given year and city index.


How to Compile and Run

Prerequisites
You will need a C++ compiler installed, such as g++.

Compilation
Open a terminal or command prompt.
Navigate to the directory where you saved weather_data.cpp.

Run the following command to compile the program:
g++ weather_data.cpp -o weather_system -std=c++11


Execution
After successful compilation, run the program from the same terminal:

On Windows: weather_system.exe

On macOS or Linux: ./weather_system


Usage
Once running, a menu will be displayed. Enter the number for the desired operation and follow the on-screen prompts.

Weather Data Storage System
1. Insert a record
2. Delete a record
3. Retrieve a record
4. Display data (Row-Major)
5. Display data (Column-Major)
6. Exit
Enter your choice: 1
Enter year: 2028
Enter city: Bengaluru
Enter temperature: 24.5
Record inserted successfully.

