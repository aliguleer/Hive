# Hive
Hue > Hive > create db> create table> quries

Test project NY Times
Soru 1

Toplam kaç yorum yapılmıştır ?
select count(*) from newyorktimes.commentsmarch2018
	246922
Soru 2

Hangi şehirden kaç yorum yapılmıştır ?

select userlocation,count(*) from newyorktimes.commentsmarch2018 group
by userlocation

Soru 3

Kullanıcı yorumlarından olumlu olan yorumları seçiniz

select  count(*) from newyorktimes.commentsmarch2018
where status='approved'
