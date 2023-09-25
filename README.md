# BANCO-DE-DADOS

## 1. Selecione todos os dados dos países da tabela_paises;
```SQL
SELECT * FROM tabela_paises;
```
![image](https://github.com/Kelly-Romualdo/BANCO-DE-DADOS/assets/116984087/85a404af-6c24-4d63-a6dc-98896aff22fb)


## 2. Selecione todas as cidades cujo país seja brazil;
```SQL
SELECT * FROM tabela_paises WHERE pais = 'Brazil';
```

![image](https://github.com/Kelly-Romualdo/BANCO-DE-DADOS/assets/116984087/1d49d6d4-2388-4614-a78b-7d1a01265a46)


## 3. Selecione todas as cidades cuja região(estado) é ceará;
```SQL
SELECT * FROM tabela_paises WHERE regiao = 'Ceará';
```
![image](https://github.com/Kelly-Romualdo/BANCO-DE-DADOS/assets/116984087/70a4df3e-3986-43a8-b64b-3e7cf043d079)


## 4. Utilize a função count para saber quantas regiões(estados) existem na China, utilize também o group by;
```SQL
SELECT COUNT(regiao) FROM tabela_cidades WHERE pais = 'China' GROUP BY pais;
```
![image](https://github.com/Kelly-Romualdo/BANCO-DE-DADOS/assets/116984087/a138db60-e741-4903-a301-62f065761e09)


## 5. Quais regiões, diferentes, existem no Canadá?
```SQL
SELECT DISTINCT regiao FROM table_cidades WHERE pais = 'Canada';
```
![image](https://github.com/Kelly-Romualdo/BANCO-DE-DADOS/assets/116984087/a89e535f-cf4d-4731-8772-103b79b975e1)


## 6. Quantos países diferentes existem na tabela 'tabela_paises';
```SQL
SELECT COUNT(DISTINCT pais) FROM tabela_paises;
```
![image](https://github.com/Kelly-Romualdo/BANCO-DE-DADOS/assets/116984087/5483b504-178d-4b76-b835-b370807bbcfb)

## 7. Quantas cidades diferentes existem no brazil;
```SQL
SELECT COUNT(DISTINCT cidade) FROM tabela_paises WHERE pais = 'Brazil';
```
![image](https://github.com/Kelly-Romualdo/BANCO-DE-DADOS/assets/116984087/79a80836-3838-4b9e-991c-d44272ffcf02)


## 8. Selecione os países e quantas regiões cada país possui;
```SQL
SELECT pais, COUNT(DISTINCT regiao) FROM tabela_paises GROUP BY pais;
```
![image](https://github.com/Kelly-Romualdo/BANCO-DE-DADOS/assets/116984087/d3d6956f-f85c-423b-ace3-176a565df62c)


## 9. Quantas pessoas com nome começando em 'João' existem no banco?
```SQL
SELECT COUNT(*) FROM tabela_paises WHERE nome LIKE 'João%';
```
![image](https://github.com/Kelly-Romualdo/BANCO-DE-DADOS/assets/116984087/c6d969b2-4f1c-4911-b8e2-fd37c54ac197)


## 10. Quantas pessoas têm o nome John?
```SQL
SELECT COUNT(*) FROM tabela_paises WHERE nome = 'John';
```
![image](https://github.com/Kelly-Romualdo/BANCO-DE-DADOS/assets/116984087/fe84dc65-5807-4dab-a8e3-ec0e3a846911)


## 11. Ordene os nomes dos países sem repetição em ordem alfabética
```SQL
SELECT DISTINCT pais FROM tabela_paises ORDER BY pais;
```
![image](https://github.com/Kelly-Romualdo/BANCO-DE-DADOS/assets/116984087/47232187-f50b-4ca0-af51-e2154133094a)
























