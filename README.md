## Créer la database projetHotel
CREATE DATABASE projethotel character set 'utf8';

-------------------------

SHOW databases;

-------------------------

## Utiliser la database projetHotel
USE projetHotel;

-------------------------

## Créer la table hotel avec une PK id
CREATE TABLE hotel (
	id INT NOT NULL AUTO_INCREMENT,
	nom VARCHAR(50) NOT NULL,
	nb_etoile INT NOT NULL,
	PRIMARY KEY ( id )
);

![alt-text](https://github.com/Dolois/sql_requetes/blob/master/créer%20la%20table%20hotel%20de%20la%20database%20projetHotel.png)
![alt-text](https://github.com/Dolois/sql_requetes/blob/master/créer%20la%20table%20hotel%20de%20la%20database%20projetHotel%20validation.png)

-------------------------

SHOW tables;

![alt-text](https://github.com/Dolois/sql_requetes/blob/master/afficher%20les%20tables%20de%20la%20database%20projetHotel.png)

-------------------------

## Insérer une première occurence dans la table hotel
INSERT INTO hotel (id, nom, nb_etoile) VALUES
(1, ' Hotel Georges V', 5) ;
![alt-text](https://github.com/Dolois/sql_requetes/blob/master/insérer%20une%20première%20occurence%20dans%20la%20table%20hotel.png)

-------------------------

## Insérer une deuxième occurence dans la table hotel
INSERT INTO hotel (id, nom, nb_etoile) VALUES
(1, ' Hotel Mandarin Oriental', 7) ;
![alt-text](https://github.com/Dolois/sql_requetes/blob/master/insérer%20une%20deuxième%20occurence%20dans%20la%20table%20hotel.png)

-------------------------

## Lister les deux occurences de la table hotel
SELECT * FROM hotel;

![alt-text](https://github.com/Dolois/sql_requetes/blob/master/lister%20les%20deux%20occurences%20de%20la%20table%20hotel.png)

-------------------------

## nombre d'occurences dans la table hotel
Select count(*) FROM hotel;

![alt-text](https://github.com/Dolois/sql_requetes/blob/master/nombre%20d'occurences%20dans%20la%20table%20hotel.png)

-------------------------

## Sélectionner la première occurence de la table hotel
SELECT * FROM hotel WHERE id = 1;

![alt-text](https://github.com/Dolois/sql_requetes/blob/master/selectionner%20la%20première%20occurence%20de%20la%20table%20hotel.bmp)

-------------------------

## Sélectionner la deuxième occurence de la table hotel
SELECT * FROM hotel WHERE id = 2;

![alt-text](https://github.com/Dolois/sql_requetes/blob/master/selectionner%20la%20deuxième%20occurence%20de%20la%20table%20hotel.png)

-------------------------

## Supprimer la table hotel
DROP TABLE hotel;

-------------------------

## Supprimer la database projetHotel
DROP DATABASE projetHotel;




