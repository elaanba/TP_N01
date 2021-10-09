TDI : OFPPT CFIJ ALKARIA TDI 201
Développement d’application client serveur
TPN° 1 :

Soit la base de données STOCK avec une seul table produit :
•	Produit (Id_Produit, Nom, Prix, Quantité)
•	Ci-dessous le code  SQL pour la création de notre table produit dans la base produit
use master
create database STOCK
go
------------------------------------------
use STOCK
go
------------------------------------------
/* Creation du table */
create table Produit
(
Id_Produit varchar(10) primary key,
Nom varchar(20),
Prix int,
Quantité int
)
Go
/* Insertion des données */

insert into produit values
(100, 'Clavier', 50, 23),
(101, 'ProBook', 4500, 200),
('102', 'EliteBooK',2400,34),
('103', 'Z400', 2800, 29),
('104', 'Modem', 70, 70),
('105', 'USB', 30, 46)
go


1-	Connecter sur le gestionnaire SQL server et créer la base stock.
2-	Connecter sur Visual studio et récupérer la chaine de connexion en utilisant le menu explorateur des serveurs.
3-	Faire la conception du formulaire principale, qui permet le chargement de la liste de tous les produits dans un DataGridView :
a)	Initialiser la chaine de connexion avec les paramètres de connexion
b)	Créer l’objet connexion de type sqlConnection
c)	Créer un objet de type sqlcommand
d)	Ecrire et tester votre commande dans le gestionnaire de base données.
e)	Ouvrir une connexion vers la base Stock avec la méthode open().
f)	Créer un objet de type DataReader pour stocker les résultats de la commande
g)	Charger les données dans un objet datagridView 
4-	Programmer les deux butons :
-	Vider : permet d’effacer tous les textBox
-	Fermer : permet de fermer la connexion et fermer le formulaire en affichant un message de confirmation.
