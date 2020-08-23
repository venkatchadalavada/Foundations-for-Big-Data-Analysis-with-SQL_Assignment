# Foundations-for-Big-Data-Analysis-with-SQL_Assignment
This is a peer graded assignment completed as a part of Foundations for Big Data Analysis with SQL course work on Cloudera. The assignment involves working on a hands-on environment, Hue (an open source project in our big data environment that acts as a web page over a lot of other useful applications like Impala and Hive). 
For this assessment, I used Hue to examine the fun database tables and produce a database overview document.
The overview document explores the data in a database that you can subsequently use for analysis.
The document  created can help others quickly gain an overview of the data available in the database,
and it can also help you whenever you return to this database after some time away.


Fun Database Overview

Name:		venkat chadalavada
Date:		2020-08-23
===

Database:	fun
===

Notes:
1.
Column and table descriptions are estimates based on examination of the
tables, not descriptions from the data sources.
2.
Column descriptions of PK, FK, and references are descriptions of assumed
relationships between tables, not database constraints.
===

Tables:	card_rank 		
		card_suit 		
		games 		
		inventory 		
===

Table:		card_rank 

Columns (2)
  	  	Name 		Type 		Comment
1 		rank 		string 		PK, Includes null 
2 		value 		tinyint 	

Sample
  		rank 		value
1 		Ace 		NULL
2 		2 		2
3 		3 		3
===







Table:		card_suit 

Columns (2)	
  	  	Name 		Type 		Comment
1 		suit 		string 		PK
2 		color 		string 	

Sample
  		suit 		color
1 		Clubs 		Black
2 		Diamonds 	Red
3 		Hearts 		Red
===

Table:		games

 Columns (8)
  	  	Name 		Type 		Comment
1 		id 		int 		PK
2 		name 		string 		FK,inventory.game 
3 		inventor 	string 	
4 		year 		string 	
5 		min_age 	tinyint
6 		min_players 	tinyint 	
7 		max_players 	tinyint 	
8 		list_price 	decimal(5,2) 	
Sample
  


id
name
inventor
year
min_age
min-players
max_players
list_price
1
1
Monopoly 
Elizabeth Magie
1903
8
2
6
19.99


2
2
Scrabble 
Alfred Mosher Butts 
1938 
8
2
4
17.99


3
3
Clue 	
Anthony E. Pratt 
1944
8
2
6
9.99



===

Table:		inventory

 Columns (5)
  	  	Name 		Type 			Comment
1 		shop 		string 	
2 		game 		string 			PK
3 		qty 		int 	
4 		aisle 		tinyint 			Includes null 
5 		price 		decimal(5,2) 		

Sample
  		shop 		game 		qty 		aisle 		price
1 		Dicey 		Monopoly 	7 		3 		17.99
2 		Dicey 		Clue 		3 		NULL 		9.99
3 		Board 'Em 	Monopoly 	11 		2 		25.00







