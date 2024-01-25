This is a webscarpping project using python and pandas. 
I tried scarpping the booking.com webpage that has the hotels details for banff , canada
the libraries used are as follows,
import requests
from bs4 import BeautifulSoup as soup
import pandas as pd
import csv
I have scarpped the hotel name , ratings, reviews and price from the booking.com webpage suing the class name.
Eventually I stored the result in a variable and conerted it to a dataframe.
Then concatinated the dataframes together into a new dataframe variable.
Since the project is done in google collab , inorder to store the data in the google drive I have first mounted the drive
using this statement,
from google.colab import drive
drive.mount('drive')
Then converted and saved the scrapped data in to a csv file in my google drive, using the below statement,
frames.to_csv('hotels.csv')
!cp hotels.csv "drive/My Drive/"
