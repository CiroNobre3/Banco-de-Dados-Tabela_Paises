# Resolução exercício SQL
 
<h2>1ª Questão</h2>

Selecione todos os dados dos países da tabela_paises

```select * from tabela_paises;```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/442a27a5-0802-456b-ac01-bba6297ebd72)


<h2>2ª Questão</h2>

Selecione todas as cidades cujo país seja brazil;

```select cidade from tabela_paises where pais = 'Brazil';```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/745a2766-2579-45c6-b65c-505329ff949e)


<h2>3ª Questão</h2>

Selecione todas as cidades cuja região (estado) é ceará;

```select cidade from tabela_paises where regiao = 'Ceará';```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/982a4751-9740-4877-9f50-24210cf4fa81)


<h2>4ª Questão</h2>

Utilize a função count para saber quantas regiões (estados) existem na China, utilize também o group by;

```select count(*) as 'Total de regioes' from tabela_paises where pais = 'China' group by pais;```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/7dfc1853-6b61-464f-9c0a-4ed0d12fe20a)


<h2>5ª Questão</h2>

Quais regiões, diferentes, existem no Canadá?

```select distinct regiao from tabela_paises where pais = 'Canada';```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/24a02c58-a6b4-4dca-a3eb-72850e388f7a)


<h2>6ª Questão</h2>

Quantos países diferentes existem na tabela 'tabela_paises';

```select count(distinct pais) from tabela_paises;```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/c36eae0b-36b7-4f12-837d-1605335a80bc)


<h2>7ª Questão</h2>

Quantas cidades diferentes existem no brazil;

```select count(distinct cidade) from tabela_paises where pais = "Brazil";```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/1e3d0a03-2e5d-492f-b73b-3615e4952c10)


<h2>8ª Questão</h2>

Selecione os países e quantas regiões cada país possui;

```select pais, count(*) as estados from tabela_paises group by pais;```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/99bc55e8-67ee-4a9c-90f7-ab936e1209dc)


<h2>9ª Questão</h2>

Quantas pessoas com nome começando em 'João' existem no banco?

```select count(*) as 'Quantidade de João' from tabela_paises where nome = 'João';```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/dc5281f0-9be8-43c1-b4ca-2acfa84c479a)


<h2>10ª Questão</h2>

Quantas pessoas têm o nome John?

```select count(*) as 'Quantidade de John' from tabela_paises where nome = 'John';```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/8fa7245c-83d9-41d1-b2cd-0928f52ecbb3)


<h2>11ª Questão</h2>

Ordene os nomes dos países sem repetição em ordem alfabética;

```select distinct pais from tabela_paises group by pais;```

<h2>Resultado esperado</h2>

select distinct pais from tabela_paises group by pais;
