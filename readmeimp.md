# mongo-with-admin-ui
Learn mongo and mongo-express. A project for launching docker based mongodb and admin ui (browser based) for learning basics of mongo db.


## Mongo Import
  
  mongoimport --db DATABASE --c COLLECTION --file FILE --upsertFields EIN --headerline --type csv
  
  ex.  mongoimport --db IRS_Files -c NM_File --file eo_nm2.csv --upsertFields EIN --headerline --type csv


  ```
