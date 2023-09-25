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

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/fdc30774-8906-422a-8a20-f39e56506e21)


<h2>5ª Questão</h2>

Quais regiões, diferentes, existem no Canadá?

```select distinct regiao from tabela_paises where pais = 'Canada';```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/8f722dfd-5e01-4437-9ed2-40bf6ebd6496)


<h2>6ª Questão</h2>

Quantos países diferentes existem na tabela 'tabela_paises';

```select count(distinct pais) from tabela_paises;```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/5d5515cf-d066-4fba-9ccb-f7cbe5cf9290)


<h2>7ª Questão</h2>

Quantas cidades diferentes existem no brazil;

```select count(distinct cidade) from tabela_paises where pais = "Brazil";```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/3fa139b0-1275-4d07-b774-5a6075cf7028)


<h2>8ª Questão</h2>

Selecione os países e quantas regiões cada país possui;

```select pais, count(*) as estados from tabela_paises group by pais;```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/95ec8f55-fe39-4a21-a7bf-891376de2037)


<h2>9ª Questão</h2>

Quantas pessoas com nome começando em 'João' existem no banco?

```select count(*) as 'Quantidade de João' from tabela_paises where nome = 'João';```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/ccce799d-471b-466f-ae65-6ad9061010dc)


<h2>10ª Questão</h2>

Quantas pessoas têm o nome John?

```select count(*) as 'Quantidade de John' from tabela_paises where nome = 'John';```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/94612212-f680-41a0-95dc-c31944d1bef5)


<h2>11ª Questão</h2>

Ordene os nomes dos países sem repetição em ordem alfabética;

```select distinct pais from tabela_paises group by pais;```

<h2>Resultado esperado</h2>

![image](https://github.com/CiroNobre3/Banco-de-Dados-Tabela_Paises/assets/111638681/b772b12a-9a45-4d51-8c3b-bc56ffbba07f)
