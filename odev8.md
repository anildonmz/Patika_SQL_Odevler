# Odev 8

- **test** veritabanınızda **employee** isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.

````SQL
CREATE TABLE employee (
	id INTEGER PRIMARY KEY,
	name VARCHAR(50),
	birthday DATE,
	email VARCHAR(100)
);
````

<br>

- Oluşturduğumuz **employee** tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

````SQL
insert into employee (id, name, birthday, email) values (1, 'Flemming', '1976-08-18', 'fhurlin0@cnet.com');
insert into employee (id, name, birthday, email) values (2, 'Gilberto', '1930-02-24', 'gkobpal1@geocities.com');
insert into employee (id, name, birthday, email) values (3, 'Noble', '1927-05-26', 'nscimone2@salon.com');
insert into employee (id, name, birthday, email) values (4, 'Susana', '1921-03-21', 'sluquet3@vistaprint.com');
insert into employee (id, name, birthday, email) values (5, 'Rancell', '1927-08-03', 'rackenson4@hubpages.com');
insert into employee (id, name, birthday, email) values (6, 'Burgess', '1912-12-26', 'bantonellini5@jiathis.com');
insert into employee (id, name, birthday, email) values (7, 'Gwendolyn', '1957-01-08', 'gdeluce6@ucsd.edu');
insert into employee (id, name, birthday, email) values (8, 'Mellicent', '1987-03-06', 'mbalmadier7@homestead.com');
insert into employee (id, name, birthday, email) values (9, 'Joseph', '1964-01-14', 'jschulkins8@harvard.edu');
insert into employee (id, name, birthday, email) values (10, 'Beverly', '1943-09-29', 'bdalyell9@feedburner.com');
insert into employee (id, name, birthday, email) values (11, 'Leila', '1967-03-03', 'lministera@ihg.com');
insert into employee (id, name, birthday, email) values (12, 'Selina', '1973-12-13', 'sgarrattyb@ocn.ne.jp');
insert into employee (id, name, birthday, email) values (13, 'Ranice', '1963-02-26', 'rforgec@redcross.org');
insert into employee (id, name, birthday, email) values (14, 'Mariejeanne', '1936-06-15', 'mgionettittid@gnu.org');
insert into employee (id, name, birthday, email) values (15, 'Rene', '1993-06-24', 'rhandline@uiuc.edu');
insert into employee (id, name, birthday, email) values (16, 'Isadore', '1929-08-07', 'ihellisf@huffingtonpost.com');
insert into employee (id, name, birthday, email) values (17, 'Addy', '1948-12-10', 'alarringtong@dedecms.com');
insert into employee (id, name, birthday, email) values (18, 'Hilly', '1972-06-08', 'hpordalh@quantcast.com');
insert into employee (id, name, birthday, email) values (19, 'Eugenie', '1986-03-01', 'epicfordi@ask.com');
insert into employee (id, name, birthday, email) values (20, 'Katey', '1941-02-27', 'kmossopj@blogtalkradio.com');
insert into employee (id, name, birthday, email) values (21, 'Gwenette', '1987-08-05', 'gfranzelinik@1688.com');
insert into employee (id, name, birthday, email) values (22, 'Jessa', '1978-07-12', 'jcasol@umn.edu');
insert into employee (id, name, birthday, email) values (23, 'Phil', '1973-09-17', 'ptourmellm@blogs.com');
insert into employee (id, name, birthday, email) values (24, 'Joscelin', '1959-09-09', 'jgodehardsfn@printfriendly.com');
insert into employee (id, name, birthday, email) values (25, 'Hesther', '1986-06-12', 'hgiacopelloo@issuu.com');
insert into employee (id, name, birthday, email) values (26, 'Cherrita', '1904-02-18', 'ckordasp@indiatimes.com');
insert into employee (id, name, birthday, email) values (27, 'Finlay', '1903-01-02', 'fdunsfordq@nature.com');
insert into employee (id, name, birthday, email) values (28, 'Tabbi', '1940-04-28', 'tingreer@networksolutions.com');
insert into employee (id, name, birthday, email) values (29, 'Francoise', '1900-01-25', 'flamberts@foxnews.com');
insert into employee (id, name, birthday, email) values (30, 'Alysia', '1985-07-18', 'aquestet@google.es');
insert into employee (id, name, birthday, email) values (31, 'Alika', '1936-06-08', 'asonscheinu@1und1.de');
insert into employee (id, name, birthday, email) values (32, 'Etan', '1908-02-27', 'echekev@deviantart.com');
insert into employee (id, name, birthday, email) values (33, 'Steven', '1947-10-12', 'sburrettw@tiny.cc');
insert into employee (id, name, birthday, email) values (34, 'Maritsa', '1978-02-07', 'mskellernx@quantcast.com');
insert into employee (id, name, birthday, email) values (35, 'Hedvig', '1990-08-01', 'hhavilley@ft.com');
insert into employee (id, name, birthday, email) values (36, 'Sander', '1910-03-28', 'sdallmannz@hp.com');
insert into employee (id, name, birthday, email) values (37, 'Vanessa', '1987-09-13', 'vpannaman10@github.com');
insert into employee (id, name, birthday, email) values (38, 'Kassandra', '1964-02-28', 'khugonet11@google.it');
insert into employee (id, name, birthday, email) values (39, 'Glennie', '1906-07-05', 'gfinder12@furl.net');
insert into employee (id, name, birthday, email) values (40, 'Linus', '1984-01-06', 'lpadberry13@apache.org');
insert into employee (id, name, birthday, email) values (41, 'Susanna', '1942-05-06', 'snorthcott14@fema.gov');
insert into employee (id, name, birthday, email) values (42, 'Kimberley', '1914-11-26', 'koleksinski15@squidoo.com');
insert into employee (id, name, birthday, email) values (43, 'D''arcy', '1993-11-07', 'dstapylton16@blinklist.com');
insert into employee (id, name, birthday, email) values (44, 'Elena', '1900-03-05', 'easgodby17@webmd.com');
insert into employee (id, name, birthday, email) values (45, 'Ignacio', '1919-01-24', 'isedger18@senate.gov');
insert into employee (id, name, birthday, email) values (46, 'Maurita', '1901-11-16', 'mliebermann19@xinhuanet.com');
insert into employee (id, name, birthday, email) values (47, 'Preston', '1960-08-09', 'pwhisker1a@nhs.uk');
insert into employee (id, name, birthday, email) values (48, 'Goran', '1963-02-04', 'goosthoutdevree1b@fda.gov');
insert into employee (id, name, birthday, email) values (49, 'Lisle', '1921-01-19', 'lledger1c@independent.co.uk');
insert into employee (id, name, birthday, email) values (50, 'Barnett', '1996-10-22', 'bmaleney1d@mlb.com');
````

<br>

- Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

````SQL
UPDATE employee
SET name = 'Fhurlin'
WHERE id = 1;

UPDATE employee
SET name = 'Gwen',
	email ='gwend6@ucsd.edu'
WHERE id = 7;

UPDATE employee
SET birthday = '1990-12-13'
WHERE name = 'Selina';

UPDATE employee
SET name = 'Holi'
WHERE name = 'Hesther';

UPDATE employee
SET birthday = '1950-01-25'
WHERE id = 29;
````

<br>

- Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

````SQL
DELETE FROM employee
WHERE id = 50;

DELETE FROM employee
WHERE name = 'Goran';

DELETE FROM employee
WHERE email = 'pwhisker1a@nhs.uk';

DELETE FROM employee
WHERE name LIKE '%a%b%c';

DELETE FROM employee
WHERE name LIKE '_a%';
````

<br>

[Patika.dev için tıklayınız](https://app.patika.dev/moduller/sql/Odev8)