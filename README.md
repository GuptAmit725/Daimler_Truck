
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
  

  
Steps to solve the task 1: 
    1.create an instance of the class ETL.
        etl = ETL()
        
    2.Load the original unprocessed data by calling load_data function from ETL class.
        raw_data = etl.load_data(path)
        
    3.Load the processed data by calling the function getData from ETL class.
      This function requires two attributes which are the paths for two datasets vehicle_data and vehicle_hash.
         processed_data = etl.getData(path_vehicle_data,path_vehicle_hash)
    
    4. Save the processed data by calling saveData function from ETL class.
         etl.saveData(data_to_be_saved, path_to_save)
         
         Note : if path is not passes anything then the data is automatically saved in current working directory.
  
  
  
  Note : To solve the task 2 questions, we will be using the preprocessed data from task 1.



Steps to solve :
    1. create an instance of EDA class with passing preprocessed data as init attribute.
            eda = EDA(preprocessed_data)
            
    2. To answer 2.1, call the function 'top_buying_countries' with start and end date between which you want see the sales.
            eda.top_buying_countries(start_date,end_date,top_n)
            
       Note : This gives us the top buying coutry and nice beautifull plot to visualize the the distribution. top_n is optional
              attributes and could be changed as per the user. 
       
            
    3. To answer 2.2 call the function 'best_seeling_year', this shows the output as bar plot top selling year arranged in
       descnding order.
            eda.best_selling_year()
    
    4. To answer 2.3 the FIN for the very first sold vehicle, call the 'get_fin_for_first_truch_sold' function that's it.
            eda.get_fin_for_first_truck_sold()
            
    5. To answer 2.4, vehicle sold with certain engines in a range of date. Call the function   'vehicle_sold_with_certain_engines' with an engine data as attribute.
            engine_data = etl.load_data(engine_data_path)
            eda.vehicle_sold_with_certain_engines(engine_data)
            
    6. To answer 2.5, same above function is used with different name and with two additional attributes as q5 and country.
            eda.get_fin_with_contry_and_date_range(engine_data)
            
       Note : Make sure engine data is loaded if note the use engine_data = etl.load_data(engine_data_path) before executing above line of code.
    
