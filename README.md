# AtividadeSQL
SQL

1. Selecione todos os dados dos países da tabela_paises;

   select * from tabela_paises;

![imagem](https://github.com/regilanenascimento/AtividadeSQL/assets/117529030/ef1c4e9e-39a1-4220-bdc0-de13a6ba83bd)


2. Selecione todas as cidades cujo país seja brazil;

   select cidade from tabela_paises where pais = 'Brazil';
   
![imagem02](https://github.com/regilanenascimento/AtividadeSQL/assets/117529030/78b957cb-4f1e-4c39-b29a-b03e93e7a98d)


3. Selecione todas as cidades cuja região(estado) é ceará;

   select * from tabela_paises where regiao = 'Ceará';

![imagem03](https://github.com/regilanenascimento/AtividadeSQL/assets/117529030/983e7ece-2950-4c0c-9b41-f44400c3a71c)


4. Utilize a função count para saber quantas regiões(estados) existem na China, utilize também o group by;

   select count(regiao), regiao from tabela_paises where pais = 'China' group by regiao;

![imagem04](https://github.com/regilanenascimento/AtividadeSQL/assets/117529030/c6bf6744-7370-4643-bbe0-e485cc1e4b08)


5. Quais regiões, diferentes, existem no Canadá?

   select regiao from tabela_paises where pais = 'Canada';

![imagem05](https://github.com/regilanenascimento/AtividadeSQL/assets/117529030/81a6bb91-bc3e-408c-9dcd-85ec511ded87)



6. Quantos países diferentes existem na tabela 'tabela_paises';

   select count(distinct pais) from tabela_paises;

![imagem06](https://github.com/regilanenascimento/AtividadeSQL/assets/117529030/259a900f-2be8-4093-9da1-b67884f61549)



7. Quantas cidades diferentes existem no brazil;

    select count (distinct cidade) from tabela_paises where pais = 'Brazil';

![imagem07](https://github.com/regilanenascimento/AtividadeSQL/assets/117529030/a6e608c3-fd98-465e-9b9a-f5e9b1c3f77b)


8. Selecione os países e quantas regiões cada país possui;

   select pais, count (distinct regiao) from tabela_paises group by pais;

![imagem08](https://github.com/regilanenascimento/AtividadeSQL/assets/117529030/42f0b33a-e553-45a5-b0b9-88c8928de4d5)


9. Quantas pessoas com nome começando em 'João' existem no banco?

   select count(nome) from tabela_paises where nome like '%Joao%';

![imagem09](https://github.com/regilanenascimento/AtividadeSQL/assets/117529030/c013d40b-df03-4ddd-9e67-3b005437b362)


10. Quantas pessoas têm o nome John?

    select count(nome) from tabela_paises where nome like 'John%';

![imagem10](https://github.com/regilanenascimento/AtividadeSQL/assets/117529030/a82823a9-70d2-4a78-b7d3-f8323a59682b)



11. Ordene os nomes dos países sem repetição em ordem alfabética;

    select pais from tabela_paises group by pais order by pais;

![imagem11](https://github.com/regilanenascimento/AtividadeSQL/assets/117529030/5e54123b-90a8-49a2-bbdb-71e773086c2b)
