## Créer la database projetHotel
CREATE DATABASE projethotel character set 'utf8';

SHOW databases;

## Connecter à la database projetHotel
USE projetHotel;

## Créer la table hotel avec une PK id
CREATE TABLE hotel (
	id INT NOT NULL AUTO_INCREMENT,
	nom VARCHAR(50) NOT NULL,
	nb_etoile INT NOT NULL,
	PRIMARY KEY ( id )
);

SHOW tables;

## Insérer une première occurence dans la table hotel
INSERT INTO hotel (id, nom, nb_etoile) VALUES
(1, ' Hotel Georges V', 5) ;

## Insérer une deuxième occurence dans la table hotel
INSERT INTO hotel (id, nom, nb_etoile) VALUES
(1, ' Hotel Mandarin Oriental', 7) ;

## Lister les deux occurences de la table hotel
SELECT * FROM hotel;

## nombre d'occurences dans la table hotel
SELECT count(*) FROM hotel;

## Sélectionner la première occurence de la table hotel
SELECT * FROM hotel WHERE id = 1;
![alt-text](https://github.com/Dolois/sql_requetes/blob/master/selectionner%20la%20première%20occurence%20de%20la%20table%20hotel.bmp)

## Sélectionner la deuxième occurence de la table hotel
SELECT * FROM hotel WHERE id = 2;
![alt-text](https://github.com/Dolois/sql_requetes/blob/master/selectionner%20la%20deuxième%20occurence%20de%20la%20table%20hotel.png)


## Supprimer la table hotel
DROP TABLE hotel;

## Supprimer la database projetHotel
DROP DATABASE projetHotel;




