It may happen with pandas in #python when use read_csv, it shows an error like this: 

AttributeError: 'float' object has no attribute 'split' 
 
 
.split() uses just for text, but it shows the column has other data types, so the code need .astype(str) after data frame.
