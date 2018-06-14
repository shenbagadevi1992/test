1.select h.hotel_no,h.name,h.city,r.room_no,r.type,r.price from hotel h join room r on h.hotel_no=r.hotel_no;

2.select h.hotel_no,h.name,h.city,r.room_no,r.type,r.price from hotel h join room r on h.hotel_no=r.hotel_no and h.city='new york'

3.select name,city from guest order by city;

4.select * from room where hotel_type='N'order by price;

5.select count(*) as "no of hotels" from hotel;

6.select distinct(city) from from guest;

7.select avg(price)as "average price of a room" from room;

8.select h.name,r.room_no,r.type from hotel h join room r on r.hotel_no= h.hotel_no;

9.select h.name,b.date_from,b.date_to,b.room_no from hotel h join booking b on h.hotel_no=b.hotel_no and city="new york"

10.select count(*) from booking where date_from='SEP';

11.

12.select h.name,r.room_no from room r join hotel h on r.hotel_no= h.hotel_no not in (select room_no from booking);

13.select h.name,h.city from hotel h join room r on h.hotel_no= r.hotel_no where price in (select max(price) from room );

14.

15 select city,avg(price) from room r join hotel h on h.hotel_no= r.hotel_no group by 'city';
