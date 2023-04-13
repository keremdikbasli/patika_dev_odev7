# patika_dev_odev7

1-) Film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.
    SELECT rating, COUNT(*) FROM film GROUP BY rating;
    
2-) Film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.

    SELECT replacement_cost, COUNT(*) AS film_sayisi 
    FROM film 
    GROUP BY replacement_cost 
    HAVING COUNT(*) > 50 
    ORDER BY film_sayisi DESC;
    
3-) Customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir?

    SELECT store_id, COUNT(*) AS customer_sayisi FROM customer GROUP BY store_id;
