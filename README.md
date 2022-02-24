### Sobre a InCicle

A InCicle é uma empresa de tecnologia com foco em soluções para sistemas de gestão, recursos humanos e relacionamentos profissionais.

### Teste Backend

Esse teste consiste em conhecermos um pouco o seu conhecimento na área de desenvolvimento de **apis rest**.
Sendo assim, avaliaremos o seu domínio das linguagem Php ^8.x utilizando o framework Laravel ^8.x ou ^9.x.

### Tarefa 1

Criar um banco de dados contendo informações dos estados e cidades do Brasil. Deixe em anexo o sql do banco. Pode usar tanto POSTGRESQL como NOSQL e utilizar o ORM Eloquent disponível no Laravel nas consultas. Neste mesmo banco crie uma tabela de pessoa com os campos nome, cpf, estado e cidade. Também criar uma tabela de log, colocando os campos: função usada, ação, hora e data

### Tarefa 2

Desenvolva uma api com os seguintes controllers,

Cadastro das cidades de um estado. Listagem das cidades de um estado usando paginação nos dados. Criar uma função para inserir novas cidades. Criar uma função para atualizar novas cidades. Criar um endpoint para verificar se a cidade existe. Desenvolver Testes Unitários das tarefas acima com phpUnit ou PestPhp.

### Tarefa 3

Crie uma api que colete dados de uma pessoa como nome, cpf, estado e cidade e faça a inserção na tabela do banco pessoa. Essa api tem que consumir a outra api da tarefa 2 para validar se a cidade que usuário colocou tem no banco de dados.

### Tarefa 4

Desenvolver uma api com WebSocket, conectando as duas apis desenvolvidas nas tarefas 2 e 3 que colete informações em tempo real de uma ação feita, e insira na tabela de logs.

### O que iremos avaliar:
- A organização do seu projeto, e a forma que seu código foi escrito.
- Se a sua solução atende tudo que foi solicitado.
- Se preocupou com performance da aplicação.
- O código é fácil de dar manutenção.
- Cobertura de código >= a 70%.
- Você entregou um readme com tudo que precisamos para executar.

### Itens que nos deixam com mais vontade de ter você no nosso time:

- Seu repositório contém algum tipo de script que cria o bando de dados e toda a “infra” necessária para a execução.
- Você foi além, e conseguimos testar a aplicação acessando uma versão que você deixou rodando em algum host público.
- Você foi mais além ainda, e conseguimos rodar localmente apenas baixando uma imagem docker ou dando um docker-compose up.
- Seu repositório tem algum tipo de automação compile o projeto e rode os testes.
- A sua API possui documentação (eu li swagger?)

### Envio

- Realizar o dump da base de dados e enviar em conjunto com os dados do projeto para um repositório publico no github com nome **Teste Backend InCicle** e envie o link para <recrutamento@incicle.com> seu nome completo no corpo do email.
