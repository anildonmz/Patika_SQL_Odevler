# Odev 12

Aşağıdaki sorgu senaryolarını **dvdrental** örnek veri tabanı üzerinden gerçekleştiriniz.

- **film** tablosunda film uzunluğu **length** sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?

````SQL
SELECT COUNT(*) FROM film
WHERE length > 
(SELECT AVG(length) FROM film);
````

<br>

- **film** tablosunda en yüksek rental_rate değerine sahip kaç tane film vardır?

````SQL
SELECT COUNT(*) FROM film
WHERE rental_rate =
(SELECT MAX(rental_rate) FROM film);
````

<br>

- **film** tablosunda en düşük rental_rate ve en düşük replacement_cost değerlerine sahip filmleri sıralayınız.

````SQL
SELECT title, rental_rate, replacement_cost FROM film
WHERE (rental_rate,replacement_cost) = 
(SELECT MIN(rental_rate), MIN(replacement_cost) FROM film);
````

<br> 

- **payment** tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.

````SQL
SELECT customer_id, first_name, last_name, 
(SELECT COUNT(*) FROM payment WHERE payment.customer_id=customer.customer_id) as times 
FROM customer
ORDER BY times DESC;
````

````SQL
SELECT  first_name, last_name, COUNT(*) FROM customer
INNER JOIN payment ON customer.customer_id = payment.customer_id
GROUP BY first_name, last_name
ORDER BY COUNT(*) DESC;
````

<br>

[Patika.dev için tıklayınız](https://app.patika.dev/moduller/sql/Odev12)
