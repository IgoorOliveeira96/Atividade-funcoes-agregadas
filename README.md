# Atividade-funcoes-agregadas

Atividade banco de dados

1- SELECT MAX(total) AS'TOTAL', MAX(hp) AS 'HP', MAX(ataque) AS 'ATAQUE', MAX(defesa) AS 'DEFESA', MAX(ataque_especial) AS 'ATAQUE ESPECIAL', 
MAX(defesa_especial) AS 'DEFESA ESPECIAL', MAX(velocidade) AS 'VELOCIDADE', MAX(taxa_captura) AS 'TAXA CAPTURA'
FROM pokemon;


SELECT MIN(total) AS'TOTAL', MIN(hp) AS 'HP', MIN(ataque) AS 'ATAQUE', MIN(defesa) AS 'DEFESA', MIN(ataque_especial) AS 'ATAQUE ESPECIAL', 
MIN(defesa_especial) AS 'DEFESA ESPECIAL', MIN(velocidade) AS 'VELOCIDADE', MIN(taxa_captura) AS 'TAXA CAPTURA'
FROM pokemon;

2- SELECT COUNT(DISTINCT cor) AS 'QUANTIDADE'
FROM pokemon;

3- SELECT AVG(peso_kg) AS 'PESO MEDIO'
FROM pokemon;

4- SELECT SUM(altura_m) AS 'ALTURA'
FROM pokemon;

5- SELECT COUNT(*) AS 'QUANTIDADE POKEMON'
FROM pokemon;

6- SELECT AVG(altura_m) AS 'ALTURA MEDIA'
FROM pokemon;

7- SELECT STD(hp) AS 'DESVIO'
FROM pokemon;

8- SELECT COUNT(tipo2) AS 'QUANTIDADE'
FROM pokemon;

9- SELECT COUNT(DISTINCT tipo1) AS 'DIFERENTES TIPOS'
FROM pokemon;

10- SELECT SUM(peso_kg) AS 'SOMA PESO'
FROM pokemon;

11- SELECT COUNT(lendario) AS 'QUANTIDADE LENDARIO' 
FROM pokemon
WHERE lendario = 1;
SELECT COUNT(lendario) AS 'NÃO LENDARIO'
FROM pokemon
WHERE lendario = 0;

	

12- SELECT cor, COUNT(*) AS 'QUANTIDADE'
FROM pokemon
GROUP BY cor
ORDER BY COUNT(*) DESC;

13- 

14-

15- SELECT AVG(taxa_captura) 
FROM pokemon
GROUP BY tipo1
HAVING AVG(taxa_captura) >100;

16- SELECT AVG(total) lendario, cor
FROM pokemon
WHERE lendario = 0
GROUP BY cor;

17-SELECT geracao, MAX(total) AS 'MAXIMO TOTAL'
FROM pokemon
GROUP BY geracao;

18- 

19- SELECT AVG(taxa_captura), geracao, tipo1, tipo2
FROM pokemon
GROUP BY geracao, tipo1, tipo2;

20- 
