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

# we can give acceess of dataset to others team members
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/5e4a8e5c-de74-4253-b2e5-90a19a78df82" />
we can give these access and add users
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/5dfc367e-1b52-4f02-9897-8d5df07febe3" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/a3cdc0e6-6b99-4bf7-999e-999139926686" />
and see the different roles and give access for project only or dataset 
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/a32f6bb1-2c33-4afd-9554-a862b21c4d94" />
see create new dataset and copy dataset
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/0e2ceca2-23b2-4c61-a153-cae63af1db1b" />
instead of dataset2 we created dataset1_copy
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/860dddd6-7856-4c39-bfce-0f08fd430e13" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/c1beb263-ae62-47c3-928b-edcbd0a46452" />
for copy dataset select the source dataset and then select copy and you will get this and mention which dataset you want to copy
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/f5a22de5-358a-44f5-8665-427a856ce8c4" />
and then click on copy the data will be copied in dataset1_copy
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/ea11e054-7d60-4a7c-b9d3-c79a773e45cb" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/1dc36c78-d922-4c28-8645-a7c1aa92ea88" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/5278ff71-d1eb-4218-97d6-d4a29d9b6f77" />
and we will see the data data copied in the dataset
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/ed1dd4d1-a62e-4d8c-af1c-f9505bcd0e08" />
copy dataset 2nd method  # transfer service for scheduling jobs seelct datatransfer option and then click on create transfer
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/ca4f93b0-ef3f-40d4-83b1-54e7a5460fa0" />
then select source dataset copy
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/d70ba039-a8a0-45fe-8b88-4f482817e991" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/c3f255aa-10b7-437c-b109-22e4d0402532" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/037733ad-63ce-4bbf-b005-3cb34bf2926d" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/dc91b94d-4845-4eee-869a-560a25eea477" />
copied
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/70738e19-083e-47dd-8ad4-ded4ab798f9b" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/06be1fec-d2c6-454f-a89d-a3c87bff2b1e" />
we can copy table click on table and then click on copy
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/8ab15278-8ebd-48a9-bc78-12f20fda1c03" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/786c897a-9c51-46ef-8935-1fb32e23c2fb" />
we can see table copied to new table auto_detect_copy_table
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/c2da9592-fb4a-4dc7-bbe4-62b9da18cb39" />
and similarly we can delete table andedit the schema
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/848f8bc2-8371-4962-abc0-5ada07d361a6" />
to change Schema click on edit schema and change and we can add new col
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/85d610d1-9dd3-4f60-aea3-6043b86f8a4e" />
but some operation we can't perform like changing the col name through UI and many more   so for this we have to change using query
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/62eb5ee0-4144-4c86-a29f-a1cfcc1fa693" />
here we can ssee count renamed ti name_coubnt
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/726140cd-4693-4826-945c-681c6aaa5a30" />
and we change data type of columns
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/fcb61be2-64ce-4159-b1ed-10a72546ba4c" />
see name count col became float
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/324218c8-d429-49b2-9ba6-5c1fdd3a53e9" />
and we can do query like this

and we restore the deleted col within time travel 
# let's delete all the rows in names table
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/44a5e36c-8c3c-4fc8-a3c6-ac7a872a84d1" />
see the table is empty
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/0b88eb7b-2363-4ac5-8737-00a9f631b14f" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/000d727a-ab25-49e9-8090-565f76b1d493" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/fdcadc02-1ddd-4568-9cb6-7d0cfc6ef10e" />
then run the written query for restore the data and we can see the data, data restored in th esame tables 
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/6618aa1d-4299-4fe7-8c8f-30f298ea355b" />
if query is not dependent then it will run paralelly
# let's see partition by ingestion time
load the data and then select 
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/3d236720-efec-4e11-8561-7d50ca1d78fe" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/19d1a4ef-540b-405d-8be6-30f0aacc95c2" />
table created
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/e7f7004e-4d60-420b-8ded-c50d79f18871" />
select legacy to run the below query
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/45d887af-eb2e-4e4f-8c1d-db1f0fe067f5" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/61ae849e-c3b0-400c-bbe8-a199bf37b1b1" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/e80c130f-78fc-4ea5-9458-05c271b07fd5" />



























































