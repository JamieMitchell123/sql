# SQL notes from software systems and how to use sql for future reference
## commands of interest:
### create file: create database <name>
- **> sqlite3 <name>**
- **> .save bookdb_new.db**
- **> .quit** (autosave)
- **> PRAGMA foreign_keys=1;** (will enforce foreign keys because theyre not automatically enforced
### example
**> CREATE TABLE Book(ISBN VARCHAR(20) PRIMARY KEY, title VARCHAR(100), author 
VARCHAR(50));** __
**> CREATE TABLE Fiction(ISBN VARCHAR(20) PRIMARY KEY, numpages INTEGER, 
genre VARCHAR(10), ispaperback INTEGER, price REAL,
FOREIGN KEY (ISBN) REFERENCES Book(ISBN)
)**  

