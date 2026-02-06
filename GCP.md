## we have to create dataset before loading the data, right click on project 3 dot and get this option create dataset and  Dataset name are case sensitive
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/5048cbc6-f19c-48cb-8909-3f49c190d895" />
and we will get a popup that set the dataset name and region, region basically means in which data center we are stroing the data and choose region correctly because cost also vary and choose nearest location
and we can set table expiration days 
and in advance option also we can see
Collation in BigQuery is a set of rules that determines how strings are sorted and compared, including rules for case sensitivity, accent sensitivity, and language-specific ordering [1]. It allows data engineers and analysts to perform culture-aware sorting and filtering operations, which is crucial for handling text data accurately across different languages and regions

<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/fad69354-c033-4a5e-8de0-b1e9229dbcb7" />
and you can see dataset ccreated 
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/7d362a08-8e50-4fa3-8f02-bbefe561c863" />
can craete unlimited datasets per project and we can craete unlimted taables but performance will reduce
now see how to create table and upload the data .  select the dataset and then select on create table
and will get multiple option if we ahve table then select upload option and upload the data using upload method have some limitation that file size must be less than 10 MB
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/f3db54top 10 mef-8466-491b-b601-1e0fa18510d6" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/be3fedc3-9d3b-490b-9de4-cdbf4a8595c8" />
and we can add field like this or just click on Schema Autodetect
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/cc9b8158-9aa0-4874-b10e-bb3215b27d57" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/6dc36a59-d5d0-478f-b91e-bd844567311c" />
and then craeet table and we can see the table craeted
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/140fffce-89ff-4314-b3ad-6e43c6f72c73" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/5fc9b961-f882-4b37-9393-4f5981510818" />
after selecting the tabe select preview option to see the data and if you want to preview the data just click on preview don't run selct * query select query will charge something
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/eb5f7ea5-e98b-4a40-9ae4-0da9c281a1fd" />
this is just one way of creating table and we have multiple way to create table 
lets run some query

top 10 male emp by count
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/bf43d887-589b-4bc7-b954-d53e38dc7cb8" />
if i run the same query again, it will not charge, it will give the cache result
click on the 3. and then more option select format to format the query
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/0e9ec52b-d28d-4725-a7de-74f4a871e8c1" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/909453ff-0647-4fe3-9556-1db9fdf8a043" />
and we can select query setting option and 
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/3b214612-7285-4009-91db-a7aa3686f096" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/94f53224-56e2-46d1-bf1d-8bb45000db8c" />














