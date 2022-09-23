# DIO_Entendendo_banco_de_dados (Documento relacionado a desafio - O Papel dos Bancos de Dados SQL e NoSQL na Engenharia de Dados)

## Banco de Dados Relacional

O conceito de Banco de Dados Relacional é um dos mais utilizados atualmente, devido a sua consistência e aplicabilidade em contextos diversos, tanto de alta complexabilidade como transações bancárias, até aplicações mais básicas como o gerenciamento de pequenos estabelecimentos comerciais.

Nesse cotexto existem diversas ferramentas que auxiliam na criação de um Banco de dados, no contexto deste curso foi utilizado o MySQL que é uma ferramenta de desenvolvimento e gerenciamento de Banco de Dados gratuita desenvolvida pela Oracle.

### Etapas importantes na criação de um Banco de Dados

Um engenheiro de Dados precisa antes de tudo entender especificamente quais as necessidades de aplicação de seu Cliente. Após este processo ele precisa define um modelo de Entidade Relacionamento para que possa começar a desenvolver de maneira mais efetiva o seu projeto.Um outro ponto é que ele de preferência precisa verificar se este modelo de Entidade Relacionamento atende adequadamente as especificações do Cliente.

A partir de então o Engenheiro de Dados pode começar a refinar mais o seu modelo como no Modelo EER, onde se definirá as classes mais detalhadamente e algumas das restrições que o Banco de Dados irá aplicar, bem como nessa Fase se tem uma visão mais detalhada da arquitetura do Projeto.

Por fim O Engenheiro de Dados irá criar de fato o Banco de Dados e assim realizar todas as suas conexões, restrições(constraints) e eventuais ajustes na arquitetura projetada para que ela se adapte da melhor forma possível a realidade da(s) aplicação(ões) que irá utilizar este Banco de Dados.

### Considerações na Criação de Banco de Dados

É importante salientar algumas considerações na hora que se está projetando um Banco de Dados.

* Atentar se é mais adequado definir uma informação como Atributo ou Categoria dependendo das relações que esta possui.
* Pensar na aplicação e quais tips de restrições seriam adequados para a aplicação, exemplo: identificar quando os atributos devem ser únicos na Tabela(Unique), definir adequadamente o tipo de variável que ela armazenará (INT, FLOAT, VARCHAR, DATE, etc)
* Pensar em nomes diretos e objetivos para a nomeação de Tabelas, atributos e Constraints, pensando nos usuários que precisaram consultar ou inserir dados nas tabelas dos Bancos de Dados.
* Avaliar se a criação das "Chaves Estrangeiras"(Foreign Keys) estão sendo feitas de forma adequada representando adequadamente os relacionamentos entre as entidades.
* Criar tabelas que não somente otimizem o armazenamento dos Dados, mas também que facilitem a busca e agregação de pessoas que possam inserir dados ,ou realizar consultas por meio da aplicação por meio de Queries.

## Banco de Dados não Relacionais

Para Aplicações que necessitam de armazenamento e Leitura de uma grande quantidade de Dados, BIG DATA, por exemplo, os Bancos de Dados Relacionais, podem não ser a adequados para se tratar destas situações. Neste contexto surgiram os Bancos de Dados não relacionais que visam garantir uma maior velocidade na leitura e armazenagem de Dados utilizando modelos que não são tão rígidos como os utilizados em Banco de Dados Relacionais, mas que para este contexto possa ser os mais adequados.

Os Bancos de Dados Não Relacionais são bem diferentes entre si e neste curso se estudo quatro categorias deste tipo de Banco de Dados:

### Banco de Dados direcionados a Grafos

Este tipo de Banco é indicado para se verificar por grafos os relacionamentos entre entidades de um mesmo contexto ou de contextos diferentes, um dos Banco de Dados mais utilizados para este tipo de aplicação é o Neo4J

### Banco de Dados Orientado a Colunas

Ideal para quando a aplicação requer uma quantidade muito maior de Leitura do que de escrita, este banco por valores nulos não serem armazenados em colunas pode economizar, um espaço considerável de armazenamento. O Software utilizado neste curso foi o Cassandra.

### Banco de Dados Direcionados a Chaves-Valor

Banco de Dados voltado para aplicações que se tem a necessidade de um monitoramento constante do tempo de criação e de uso das informações, tais como Cache, Sessão de Usuário, Carrinho de Compras e depois disto as informações são repassadas e aquele ambiente é deletado.

A Ferramenta utilizada neste curso para isso foi o REDIS.

### Banco de Dados Direcionados a Documentos

Na gestão de Documentos, principalmente documentos autocontidos (em que as informações necessárias estão nele próprio) esse tipo de Banco é um dos mais adequados, devido a sua flexibilidade, versatilidade e velocidade.
Neste curso foi explorado em um pouco mais de detalhes os comandos mais básicos do Banco de Dados MongoDB que é atualmente o mais utilizado para este tipo de aplicação.
