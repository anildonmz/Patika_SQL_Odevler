# Odev3

Aşağıdaki sorgu senaryolarını **dvdrental** örnek veri tabanı üzerinden gerçekleştiriniz.  

- **country** tablosunda bulunan **country** sütunundaki ülke isimlerinden 'A' karakteri ile başlayıp 'a' karakteri ile sonlananları sıralayınız.  

````SQL
SELECT country FROM country
WHERE country LIKE 'A%a';
````  

<br>

- **country** tablosunda bulunan **country** sütunundaki ülke isimlerinden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız.  

```` SQL
SELECT country FROM country
WHERE country LIKE '_____%n';
````  

<br>

- **film** tablosunda bulunan **title** sütunundaki film isimlerinden en az 4 adet büyük ya da küçük harf farketmesizin 'T' karakteri içeren film isimlerini sıralayınız.  

```` SQL
SELECT title FROM film
WHERE title ILIKE '%t%t%t%t';
````  
<br>

- **film** tablosunda bulunan tüm sütunlardaki verilerden **title** 'C' karakteri ile başlayan ve uzunluğu (length) 90 dan büyük olan ve rental_rate 2.99 olan verileri sıralayınız.  

```` SQL
SELECT * FROM film
WHERE title LIKE 'C%' AND length > 90 AND rental_rate=2.99;
```` 

<br>

[Patika.dev için tıklayınız](https://app.patika.dev/moduller/sql/Odev3)


