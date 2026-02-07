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

wildcard
Wildcard tables in Google BigQuery allow for querying multiple tables with similar names using a single, concise SQL statement, enhancing scalability. They use a special character (*) to represent unknown characters in table names, enabling, for example, the querying of daily, partitioned tables (table_*). 

if we want to fetch data from public we have to select on explore and select add data we will get multiple options, and we can select public datasets
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/9c7ccd0b-d1d6-4074-b442-49748e03c8a8" />

we selected this public dataset
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/5b42c110-1cf5-47e4-94b6-a08f2e8699a7" />
click on view dataset and it will load and we can use
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/f3ceafcd-2d8c-450c-893d-8cea8178a871" />
and new resource will be listed here containing many public dataset and we will seelect noaa gsod or req dataset
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/c143953a-68e6-4366-8cea-d7480676c2a9" />
and we can see the data 
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/2822c002-d785-4948-a56b-fc102da1a5ab" />
here we can see we have data from 1929 and if we run normal query to get somethis it will be very difficult and time consuiming as we have to write query select query from table 1 then table 2 . and so on the same lenthy query we can write concise using  ## wildcard ## 
let's we are trying to get maximum temp between 1950 to 1959 
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/e5da3d3b-422e-4325-9c51-5255223c2a68" />
so it will check suffix of each table which have 195 like 1950,1951 .....1959

# let we have to check for 1951 ,1952 and 1953 only 
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/fd344dd3-1dfc-43a3-892e-bee2f7fc2bcc" />
and we can save and schedule query we can enable to view the query to project team and once the query saved it will come in the saved quwry and we can share the query to anyone it will give link for query
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/6dece3be-a979-4a5e-a376-0c6879843154" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/44037eb2-8928-4c26-a006-29793952b906" />
and we can delete the dataset to avoid charge
<img width="1599" height="899" alt="image" src="https://github.com/user-attachments/assets/721e99e9-25bb-4b9f-a1a4-c23fc77ad398" />
select dataset and click on craete table then select upload and select file then file formaat and then click Schema auto detect
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/44fd538b-0d98-400f-a1ed-97c409e4b491" />
then click on create table and we ccan see the table craeted and detected format automatically
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/716b3884-8e6d-42ef-991f-a27e50b85652" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/1e7dac6b-fb27-4654-8cb3-704a27a7952d" />
but don't rely on auto-detect cross check it once
# nested_data see the schema we set
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/8e384f46-e2b4-498c-98e3-c6bf65c39153" />
see th nested table created
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/ca1924ac-bb23-4e08-9139-132171ccda81" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/b54338e0-2d39-49ef-85fa-81a99507935e" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/eed05911-bdfd-456d-ab42-ab0e8601af69" />

<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/1543d855-4dfc-4f71-92b2-ee7ab95d211b" />
and we can replace cross join by comma(,) intenally it is cross join





























