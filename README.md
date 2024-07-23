# Visualizing Credit Card Defaults using Power BI

## Overview 

This is Proof of Concept for loading, transforming and visualizing data through Power BI.

## Report Screenshot

![image](https://github.com/user-attachments/assets/2b15d145-a7ff-46fc-9ced-457cdeb90bd6)


## Tech Stack

- Power BI Desktop

## Dataset

Credit Card Defaults (UCI Machine Leaarning DataSet Repository). New Column added to original dataset (fake geo-location information for various US states).

## Solution

Firstly data is loaded into Power BI using file Data.csv. Then various transformations are applied onto original dataset. Here is the list of transformations:

![image](https://github.com/user-attachments/assets/7488ee0b-b822-41e9-91d0-0b241d49b2f1)

Then various visuals are created. For instance, in the first visual, fact is count of credit card defaults and dimensions are education level and gender. In the third visual, count of credit card defaults are being showed for each of the US states. This report is interactive which means if Texas state is being clicked in third visual then data for only Texas state is being showed in all other visuals.



