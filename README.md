# Dynamic Metadata Management
Dynamic Metadata Management is a plug-in which will help its users dynamically add new columns(data points) coming from source to the target table. It will also help handle missing columns before saving data to destination. 

## Index
- [Overview](README.md#Overview)
  - [Pre-requisites](README.md#Pre-requisites)
  - [How it works](README.md#How-it-works)
- [Credits](README.md#Credits)

## Overview
### Pre-requisites
The plug-in will require metadata about your target table. The metadata should consist of -
  1. column name
  2. column data type
  3. index  (order/placement of columns in target table)
### How it works
The metadata helps give a good understanding about the existing structure of target table. The code will then use this information to- 
- detect new datapoints/columns from source and alter the table accordingly
- detect missing records and identify what type of null value to be filled based on column data type
#### Design
- Input : 
  ```
  - Source data converted to <pandas.DataFrame>
  - Pre-requisite metadata
  ```


- Output :
  ```
  - Modified pandas dataframe to be saved at destination as table
  ```

- Process :
  
  In an ETL process, the plugin will be placed inside the transform section. Once data has been extracted from source and converted to a <pandas.DataFrame>, it will be then fed into the plug-in along with target table metadata
    ![image](https://user-images.githubusercontent.com/46084428/210352003-ddc692b1-fddc-42ed-ac26-a38686676d1f.png)
  
  [Addition of columns](#)
    - lol
    - 
2. Technologies Used
3. Challenges Faced and Features to be implemented in the future
  
## How to run the project
How to use the plugin

## Credits
> Krishna
>
> Kunal
>
> Saurav
>
> Vineet


## License (Optional)

## Badges (Optional)

## How to contibute (Optional)

## Tests
