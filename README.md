# FileFilter User Guide | v1.0
## __Program Functions__
This program acts to filter a column in a CSV file titled 'input.csv' from an inputted set of filters from 'filter.txt' and return all data within the filtered rows as a seperate CSV file named whatever the user wants it to be. 

## __Program Usage__

### <u><strong>File setup</strong></u> 
__READ AND ENFORCE BEFORE RUNNING THE PROGRAM__

Within the input file, there must be a heading for each columnm at the first row (row 1)

There also must be a text file called ___filter.txt___ that contains the filter for the program to use within the folder.
#### __Filter formatting__
Each character(s) to be filtered must be sperated by lines, with no blank line at the end (unless you want that as a filter).

_Example_: 

wang

yin

hao

lao

xing

The filter filters out all rows with 'wang', 'yin', 'hao', 'lao', and 'xing' in the selected column.

__NOTE: Capitalization does NOT matter when inputting filters or using the following functions__

### <u><strong>Filtering the input file and return its output</strong></u> 
1. Open the program
2. Input '1' to open start _Filter File_
4. Select which column in the input file to filter
5. Insert desired output file name 
6. Look in folder for the filtered output file

### <u><strong>Editing filter data</strong></u> 
While you could just open the filter file (_filter.txt_) and edit its contents manually, the program can also edit the data.

1. Open the program
2. Input '1' to open start _View/edit Filter_
3. Input '1' to open _Edit a filter_
4. Input the filter to edit | eg./ wang
5. Input new filter ot replace old filter | eg./ wan

### <u><strong>Adding a filter</strong></u> 
While you could just open the filter file (_filter.txt_) and add filters manually, the program can also add the data.

1. Open the program
2. Input '1' to open start _View/edit Filter_
3. Input '2' to open _Add a filter_
4. Input new filter to add | eg./ smith

### <u><strong>Deleting a filter</strong></u> 
While you could just open the filter file (_filter.txt_) and remove filters manually, the program can also remove the data.

1. Open the program
2. Input '1' to open start _View/edit Filter_
3. Input '3' to open _Delete a filter_
4. Input filter to delete | eg./ wang 

## __EXAMPLE:__ 

_input.csv_ :

sutdent_id | first_name | last_name | age | grade

031245 | gloria | qi | 16 | 11

452453 | alex | liu | 16 | 11

209845 | daniel | mclorey | 17 | 12

409875 | nathan | ching | 15 | 10

458035 | anna | luck | 15 | 10

349583 | jialin | qiu | 16 | 11

679283 | edeline | xie | 16 | 11

582345 | jack | smith | 16 | 10

909452 | mariam | malean | 15 | 10

_filter.txt_ :

11

12

- User selects 'grade' as column to be filtered 
    - Therefore all rows with that equal '11' or '12' within their grade column will be extracted and stored in the output csv file.

_output.csv_ :

sutdent_id | first_name | last_name | age | grade

031245 | gloria | qi | 16 | 11

452453 | alex | liu | 16 | 11

409875 | nathan | ching | 15 | 10

458035 | anna | luck | 15 | 10

349583 | jialin | qiu | 16 | 11

679283 | edeline | xie | 16 | 11
