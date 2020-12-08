# hello-world
just a repository
CREATE TABLE IF NOT EXISTS newbook_mast 
(book_id varchar(15) NOT NULL PRIMARY KEY,
book_name varchar(50)  ,
isbn_no varchar(15)  NOT NULL  ,
cate_id varchar(8)  , 
aut_id varchar(8) , 
pub_id varchar(8) ,          
dt_of_pub date ,
pub_lang varchar(15) ,
no_page decimal(5,0) ,         
book_price decimal(8,2) ,
FOREIGN KEY (aut_id) REFERENCES newauthor(aut_id));
