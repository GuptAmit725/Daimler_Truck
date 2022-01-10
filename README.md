# Description

The data to be used in this challenge can be found in the file vehicle_data.xlsx. Please 
note that the data must first be processed, i.e. it is not yet available in a quality that 
allows a final insight generation.

The source file vehicle_data.xlsx contains data for 500 vehicles. 
In the sales code tab you will find 500 trucks whose unique vehicle identification 
number (VIN) is shown as hash in the column h_vehicle_hash. Each vehicle is broken 
down by production date, country to which the vehicle was sold and sales_code_array. 
The latter column contains codes that describe the exact composition of the vehicle*. In 
the engines tab you will find 9 sales codes that tell you which engine is installed in the 
corresponding vehicle. With the table vehicle_hash you can snap the hashed VIN back into 
the original display.

The challenge is divided into two parts. The first part is aimed at your software 
development skills. Adhere to the most common clean code rules when designing the 
code and pursue test-driven development wherever possible. In the second part of the 
assignment, you will be asked to perform various analyses. Use the data you prepared in 
the first part of the assignment.

Before you start, it is a good idea to familiarize yourself with the data sets. Get an 
overview and explore the relationships of the data sets

Task 1: Data Engineering

Write an ETL pipeline for data preparation. Proceed as follows.
• Load data
• Clean and prepare data
• add data
• Save the entire table consisting of the following columns 

fin  
production_date
country
sales_code_array

Task 2: Data Science

Analyze the data by evaluating the following questions. Visualize your results.
• What are the top three countries to which we have sold arn rneist vehicles between 
  01.01.2014 and 31.12.2020.
• In which of these years did we sell the most vehicles? 
• What is the VIN of the first vehicle sold at the time.
• How many vehicles were sold between 01/01/2017 and 01/01/2021 rnith OM934, 
  OM936, OM470 and OM471 engines.
• Which vehicles (VIN) were sold to New Zealand between 01/01/2017 and 
  01/01/2021 and rnith OM936 engine
  
  
  
  
System should be WINDOWS.

Clone the github repository

1. Open gitbash or download from https://gitforwindows.org/

2. Clone the repository (command : <b>git clone https://github.com/GuptAmit725/Daimler_Truck.git )


Follow the following steps to run the file in jupyter notebook.

1. Download Anaconda if not already.(https://repo.anaconda.com/archive/Anaconda3-2021.11-Windows-x86_64.exe)

2. Open Anaconda 

3. Create new/existing env (command : <b>conda create -n env_name</b>)

4. Activate the env (command : <b>conda activate env_name</b>)

5. Open Jupyter notebook (command : <b>jupyter notebook</b>)

6. Go to github repo directory you cloned

7. Open the <b>daimler_internship.ipynb</b> file

8. Run/uncomment the command <b>!pip install -r requirements.txt</b>

9. Now run individually or at once but make sure that ETL and EDA cell are activated.
  
