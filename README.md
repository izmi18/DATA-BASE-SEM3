# DATA-BASE-SEM2
COMMAND 
PERTEMUAN 2

Creat database
CREATE DATABASE izmi_database;

Pindahin database
\c nama_database

Hapus data base 
DROP DATABASE nama_database;

Membuat table
CREATE TABLE public.user (
Id SERIAL PRIMARY KEY,
Saldo INT );

Melihat table
\dt
\d public.user

 PERTEMUAN 4

psql --username=postgres (login)
 \d user (buat liat datanya)
Untuk liat semua data
SELECT * FROM public.user

UPDATE public.user SET saldo=10000 WHERE id=1;
(buat apdate data)

  INSERT INTO public.user (nama, saldo) VALUES ('faiz amalia', 0);
(buat nambah data nama)

DELETE FROM public.user WHERE id=1;
(Untuk hapus data)

 ALTER TABLE public.provider ADD CONSTRAINT fk_user FOREIGN KEY (user_id) REFERENCES public.user(id);
ALTER TABLE
(menghubungkan table)



