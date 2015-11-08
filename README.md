# Simpla Pentaho Data Integration (Kettle) Application
## csv2ddl.ktr, tranform CSV file to DDL statement 
Execute: pan.bat /file:"<path_to_ktr_here>\csv2ddl.ktr" /param:"table_name=<table_name_here>" /level:Basic
Put <table_name_here>.csv containing column "Column Name", "Data Type", put the file in the same directory as csv2ddl.ktr. 
The generated file: <table_name_here>.txt containing DDL script 

Example:
CSV file SIMPLE_TABLE.csv
Column Name;Data Type
ID;NUMBER (38)
NAME;VARCHAR2 (6 Byte)

Output file SIMPLE_TABLE.txt
CREATE TABLE SIMPLE_TABLE (
ID NUMBER (38),
NAME VARCHAR2 (6 Byte)
);


