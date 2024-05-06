# Club-Database-Managment

1) AGE IN affiliate member should be driven
2) Entertainment type on Entertainment entity
3) Service type in services entity
4) Security entity -> deleted
5) Academy -> national_id renamed to national_id_trainer
6) Days and hours at academy -> must be at single table as its multivalue
      CREATE TABLE academy_time(
          Academy_ID INT NOT NULL,
          DAY VARCHAR(10),
          Start_hr TIME NOT NULL,
          End_hr TIME NOT NULL,
          PRIMARY KEY(Academy_ID, DAY),
          FOREIGN KEY(Academy_ID) REFERENCES academy(Academy_ID)
      );

7) Updated most of data types of attributes from of int to varchar

![image](https://github.com/MohanadKhh/Club-Database-Managment-System/assets/127995481/5cd49f10-cca4-4616-9ac0-f1cb1f4c1098)
