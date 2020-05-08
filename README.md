# Pokémon

Há mais de 10 anos, crianças do mundo inteiro vêm descobrindo o mundo encantado dos Pokémon. Hoje, a família de produtos Pokémon inclui videogames, o jogo Pokémon Estampas Ilustradas, a série de TV animada, filmes, brinquedos e muito mais. Muitos pais acreditam que o Pokémon Estampas Ilustradas e os videogames do Pokémon estimulam seus filhos a aprender a ler, já que a leitura é indispensável na maioria dos jogos do Pokémon. Os jogos também estimulam o pensamento estratégico e, em muitos casos, habilidades matemáticas básicas. O Pokémon valoriza muito o espírito esportivo e o respeito pelos outros jogadores.

## O que são Pokémon?

Pokémon são criaturas de todas as formas e tamanhos que convivem com os humanos na natureza. Na grande maioria, os Pokémon não falam, exceto para proferir seus nomes. Os Pokémon são criados e comandados por seus donos (os chamados "Treinadores"). No decorrer das aventuras, os Pokémon crescem e ganham experiência, podendo até mesmo evoluir para Pokémon mais fortes. Alguns Pokémon, como Pikachu, Piplup e Charizard, possuem papéis de destaque na série de videogames, no jogo Estampas Ilustradas e nos programas de TV, mas eles são apenas algumas das quase 500 criaturas que habitam o universo dos Pokémon.

**Fonte:** [Webiste Oficial - Pokémon](https://www.pokemon.com/br/guia-para-pais/)


## Ponto de Partida

Para começar esse exercício, você deverá: 

* 1. Pegar o arquivo `pokedex_create_v1.sql`, disponível na pasta [data](data/)
* 2. Abrir o software [MySQL](https://www.mysql.com/products/workbench/)
* 3. Exectuar o script para importar um novo banco de dados 


## Resumo do Projeto

Para este projeto, sua tarefa é criar consultas (queries), usando as técnicas da [Linguagem de Consulta de Dados](https://github.com/profdiegoaugusto/banco-dados/tree/master/mysql/linguagem-consulta-dados) no banco de dados `pokedex` do universo Pokémon. O esquema do banco de dados possui apenas uma tabela chamada `Pokémon`, com as seguintes colunas:

| Coluna          | Descrição                                                                                                                                                                                                                        |
|-----------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| numero          | Chave Primária: o número do Pokémon no Pokedex Nacional                                                                                                                                                                          |
| nome            | Nome do Pokémon                                                                                                                                                                                                                  |
| tipo1           | Todas as criaturas Pokémon e seus movimentos recebem determinados tipos. Cada tipo tem vários pontos fortes e fracos no ataque e na defesa, ou seja, cada Pokémon tem um tipo que determina sua fraqueza/resistência aos ataques |
| tipo2           | O tipo secundário do Pokémon caso ele possua                                                                                                                                                                                     |
| total           | Soma de todas as estatísticas básicas (Pontos de Vida, Ataque, Defesa, Ataque Especial, Defesa Especial e Velocidade)                                                                                                            |
| hp              | HP (Hit Points ou Health Points), define quanto dano um Pokémon pode suportar antes de desmaiar                                                                                                                                  |
| ataque          | O ataque base do Pokémon                                                                                                                                                                                                         |
| defesa          | A defesa base do Pokémon                                                                                                                                                                                                         |
| ataque_especial | O ataque especial base do Pokémon                                                                                                                                                                                                |
| defesa_especial | A defesa especial base do Pokémon                                                                                                                                                                                                |
| velocidade      | A velocidade base do Pokémon                                                                                                                                                                                                     |
| geracao         | Número da geração em que o Pokémon foi introduzido                                                                                                                                                                               |
| lendario        | Valor Booleano que indica se o Pokémon é lendário ou não                                                                                                                                                                         |
| cor             | A cor do Pokémon                                                                                                                                                                                                                 |
| altura_m        | Altura em metros do Pokémon                                                                                                                                                                                                      |
| peso_kg         | Peso em Kilos do Pokémon                                                                                                                                                                                                         |
| taxa_captura | A taxa de captura do Pokémon é um número entre 0 e 255, quanto maior, melhor |


## 1. Exercícios de Consultas


1. Selecione o banco de dados (esquema) `pokédex`.

```sql

```

2. Obtenha informações da estrutura da tabela `Pokémon`.

```sql

```

3. Selecione todos os pokémons cadastrados no banco de dados.

```sql

```

4. Selecione o `numero`, `nome`, `cor`, `altura_m` e `peso_kg` de todos os pokémons cadastrados.

```sql

```

5. Qual é o `numero` e o `nome` de todos os pokémons da primeira geração?

```sql

```

6. Quais são os pokémons `Amarelo` da primeira geração?

```sql

```

7. Qual é o pokémon mais forte?

```sql

```


8. Selecione o `numero`, `nome` e `tipo1`; de todos os pokémons cujo tipo primário é `Fire`.

```sql

```

10. Selecione em ordem decrescente o `numero`, `nome` e `defesa` de todos os pokémons.

```sql

```


11. Qual o pokémon possui *menor* taxa de captura? Selecione apenas `numero` e `nome`.

```sql

```


12. Selecione todos pokémons que não possuem tipo secundário, ou seja, `tipo2`.

```sql

```

13. Selecione `numero`, `nome`, `tipo1`, `tipo2` de todos os pokémons que possuem o peso entre 100kg e 500kg.

```sql

```


14. Crie um ranking dos top 10 pokémons mais velozes, contendo `numero`, `nome` e `velocidade`.

```sql

``` 


15. Selecione `numero`, `nome`, `tipo1`, `tipo2`, `taxa_captura` dos pokémons que possuem os dois tipos e tenham uma taxa de captura acima de 100. Ordene os resultados decrescente pela taxa de captura.

```sql

```

16. Quais são os tipos primários dos pokémons?

```sql

```

17. Selecione o `numero`, `nome` e `cor`; de todos os pokémons que o nome começa com a letra `D`.

```sql

```

18. Qual é o pokémon mais poderoso de todas as gerações?

```sql

```

19. Selecione o `numero`, `nome`, `defesa`, `ataque` dos pokémons com defesa > 60 e ataque <= 70; ordenados decrescente pelo `total`. 

```sql

```

20. Selecione todos os pokémons do tipo `Planta` e `Venenoso` que não sejam `Green`, ordenado crescente pelo `nome`.

```sql

```

21. Selecione de maneira crescente os nomes dos pokémons que possuem a letra y na 4ª posição do nome.

```sql

```

22. Qual é o maior valor de `ataque_especial` cadastrado?

```sql

```

23. Selecione o `numero`, `nome` e `altura_m` dos pokémons que possuem altura acima de 2,10m.

```sql

```

24. Quais são as diferentes tipos de cores dos pokémons? Apresente os resultados de maneira crescente pelo nome da cor.

```sql

```

25. Selecione o `nome` e `velocidade` dos pokémons com velocidade entre 30 e 70. Ordene os resultados por nome (crescente) e velocidade (decrescente)

```sql

```

26. Quem são os pokémons lendários? Apresente os resultados ordenados por `total` decrescente.

```sql

```


27. Selecione os pokémons da primeira geração com taxa de captura igual a 255.

```sql

```


28. Quem é o mais poderoso? selecione o `Pikachu`, `Squirtle`, `Bulbasaur` e `Charmander`; ordenados decrescente pelo `total`. 

```sql

```

29. Quem são os pokémons da primeira geração, que começam com a letra `d` e não possuem tipo secundário?
Ordene os resultados crescente por `taxa_captura` e decrescente pelo `total`.

```sql

```

30. Qual é o ranking dos top 5 pokémons lendários com maior `taxa_captura` e `total`? Apresente apenas `numero, nome, total, taxa_captura` nos resultados.

```sql

```

31. Selecione o `numero`, `nome`, `peso_kg` dos pokémons com peso entre 2kg e 3kgs?

```sql

```

32. Selecione o `numero`, `nome`, `tipo1` e `tipo2` dos pokémons com tipo primário `Normal`, que não possuem tipo secundário. Existe algum pokémon lendário nos resultados, se sim, os remova dos resultados?

```sql

```

33. Quem são os pokémons do tipo `Water` que não são azuis? Apresente `numero`, `nome`, `tipo1`, `tipo2` e `cor`, ordenados pelo `nome` de maneira crescente.

```sql

```

34. Crie um ranking dos top 10 pokémons mais lentos.

```sql

```

35. Selecione os pokémons cujo nome comece e termine com a letra `a`. 

```sql

```

36. Quem são os pokémons do tipo `Fire` que não são vermelhos? Apresente `numero`, `nome`, `tipo1`, `tipo2` e `cor`, ordenados pelo `nome` de maneira crescente.

```sql

```

37. Quais são os diferentes tipos de `peso_kg` dos pokémons? Apresente os resultados ordenados de maneira crescente.

```sql

```

38. Selecione o `numero`, `nome` e `hp` dos pokémons com valores entre 0 e 100. Ordene os resultados de maneira crescente por `hp` e `nome`.

```sql

```

39. Selecione o `numero`, `nome`, `hp`, `ataque`, `defesa` e `total`; dos pokémons com valores de `hp`, `ataque`, `defesa` maiores ou iguais a 100.

```sql

```

40. Selecione todos os pokémons do tipos `Water` e `Gelo`, ordenados decrescente por `total`.

```sql

```

## 2. Exercícios de Funções Agregadas

1. Quais são os valores máximo e mínimo das seguintes colunas:
    * total
    * hp
    * ataque
    * defesa
    * ataque_especial
    * defesa_especial
    * velocidade
    * taxa_captura

```sql
SELECT 
    MAX(total), MIN(total)
FROM
    pokemon;
/*--*/
SELECT 
    MAX(hp), MIN(hp)
FROM
    pokemon;
/*--*/
SELECT 
    MAX(ataque), MIN(ataque)
FROM
    pokemon;
/*--*/
SELECT 
    MAX(defesa), MIN(defesa)
FROM
    pokemon;
/*--*/
SELECT 
    MAX(ataque_especial), MIN(ataque_especial)
FROM
    pokemon;
/*--*/
SELECT 
    MAX(defesa_especial), MIN(defesa_especial)
FROM
    pokemon;
/*--*/
SELECT 
    MAX(velocidade), MIN(velocidade)
FROM
    pokemon;
/*--*/
SELECT 
    MAX(taxa_captura), MIN(taxa_captura)
FROM
    pokemon;

```

2. Quantas cores diferentes possuem os pokémons?

```sql
SELECT 
    COUNT(DISTINCT cor) AS 'cores'
FROM
    pokemon;

```

3. Qual é o peso médio dos pokémons?

```sql
SELECT 
    AVG(peso_kg)
FROM
    pokemon;

```

4. Qual é a soma das alturas dos pokémons?

```sql
SELECT 
    SUM(altura_m)
FROM
    pokemon;

```

5. Quantos pokémons estão cadastrados no banco de dados?

```sql
SELECT 
    COUNT(nome)
FROM
    pokemon;

```

6. Qual é o altura média dos pokémons?

```sql
SELECT 
    AVG(altura_m)
FROM
    pokemon;

```

7. Qual é o desvio padrão do valor de HP dos pokémons?
```sql

SELECT 
    STDDEV(hp)
FROM
    pokemon;
```

8. Quantos pokémons possuem tipo2?

```sql
SELECT 
    COUNT(tipo2)
FROM
    pokemon;

```

9. Quantos são os diferentes tipos primários dos pokémons? 

```sql
SELECT 
    COUNT(DISTINCT tipo1)
FROM
    pokemon;

```

10. Qual é a soma dos pesos dos pokémons?

```sql
SELECT 
    SUM(peso_kg)
FROM
    pokemon;


```

11. Qual é a quantidade de Pokémons lendários e não lendários

```sql
SELECT 
    lendario, COUNT(lendario)
FROM
    pokemon
GROUP BY 
	lendario;

```

12. Qual é a quantidade de pokémons para cada uma das diferentes cores ordenadas decrescente?

```sql
SELECT 
    cor, COUNT(cor)
FROM
    pokemon
GROUP BY cor
ORDER BY cor DESC;

```

13. Qual é a média de peso e altura de cada um dos tipos primários dos pokémons? Ordene os resultados decrescente respectivamente por média de peso e altura.
```sql
SELECT 
    tipo1, AVG(peso_kg), AVG(altura_m)
FROM
    pokemon
GROUP BY tipo1
ORDER BY AVG(peso_kg) DESC, AVG(altura_m) DESC;

```

14. Qual é a taxa de captura média por cor de cada um dos pokémons lendários?

```sql
SELECT 
    cor, AVG(taxa_captura) AS 'Média'
FROM
    pokemon
WHERE
    lendario = 1
GROUP BY cor;

```

15. Qual os tipos primários que possuem a taxa de captura média acima de 100

```sql
SELECT 
    tipo1, AVG(taxa_captura) AS 'Média'
FROM
    pokemon
WHERE
    taxa_captura > 100
GROUP BY tipo1;

```

16. Agrupados por cor, quais pokémons não lendários possuem média total abaixo de 400

```sql


```

17. Qual o valor máximo total em cada uma das gerações?

```sql
SELECT 
    geracao, MAX(total)
FROM
    pokemon
GROUP BY geracao;

```

18. Quantos pokémons lendários existem em cada uma das gerações?

```sql
SELECT 
    geracao, COUNT(lendario)
FROM
    pokemon
WHERE
    lendario = 1
GROUP BY geracao;

```

19. Em cada uma das gerações, quantos pokémons tem tipos primários e secundários e qual a taxa_captura média deles?

```sql
SELECT 
    geracao, COUNT(nome), AVG(taxa_captura)
FROM
    pokemon
WHERE
    tipo1 IS NOT NULL AND tipo2 IS NOT NULL
GROUP BY geracao;

```

20. Qual é a quantidade de cores de cada um dos pokémons lendários em todas as gerações?

```sql
SELECT 
    geracao, COUNT(cor)
FROM
    pokemon
WHERE
    lendario = 1
GROUP BY geracao;

```


## REFERÊNCIAS

* [Webiste Oficial - Pokémon](https://www.pokemon.com/br/guia-para-pais/)
* [Guia de Estilo SQL · SQL Style Guide](https://www.sqlstyle.guide/pt-br/)







