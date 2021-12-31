sql: structured query language  
index: a faster method to look-up and retrieve data in database  
composite index  
trigger  
partial/transitive dependency  
normalization  
denormalization  
super key: could be single or composite key  
structured data  
unstructured data  
database/database management system  
sql transaction  

ACID (transactions): 4 properties

|atomic|consistent|isolated|durable|
|------|----------|--------|-------|
|any failure will fail the entire course of transactions|total does not change after the transaction|transactions does not affect each other|database remains unchanged after the transaction|

ACID (transaction):  
- atomic: all or nothing. Any failure will fail the entire transaction
- consistent: does not change before or after transaction occurs
- isolated: does not affect other transactions
- durable: database is not affected if failure occurs

explain/desc `table`\G;  
show create table `table`  
combined index/index  
- first column counts
- if query requires more than 20% of lines, full scan is faster

select * from sys.schema_unused_indexes;  
select * from sys.schema_redundant_indexes\G;  
select * from statements_with_full_table_scans\G;  
partition:
- good for table with more than 1M lines
- no more than 50 partitions
	
