### Sobre a InCicle
A InCicle é uma empresa de tecnologia com foco em soluções para sistemas de gestão, recursos humanos e relacionamentos profissionais.
### Teste Backend
Esse teste consiste em conhecermos um pouco o seu conhecimento na área de desenvolvimento de **apis rest**.
Sendo assim, avaliaremos o seu domínio das linguagem Php ^8.x utilizando o framework Laravel ^8.x ou ^9.x ou a linguagem Type Script utilizando
o framework Adonisjs 5.
### Descrição da API
Desenvolver uma Api que atenda à modelagem disponibilizada abaixo(não necessário sem limitar a ela), está api deve ser construida com a finalidade de gerenciar atividades de um projeto que podem ser visualizadas por membros desse projeto adicionados pelo administrador.

### DIAGRAMA

![Diagrama](https://github.com/InCicle/backend-test/blob/main/DER-testes.png?raw=true)

### **Requisitos**
## item 1
Essa api deve trabalhar com autorização para somente membros poderem gerenciar as atividades.
## item 2
Deve existir dois tipos de membros, membros comuns que tem permissão somente para gerenciar atividades e tópicos e os membros administradores que tem permissão de gerenciar todas as entidades com exceção da entidade person.
## item 3
Como apresentado no diagrama as atividades ficam agrupadas em tópicos, onde possuem um campo chamado **index_on** ordenado em ordem crescente (0,1,2,3,4...) que guarda a sua posição da atividade dentro do tópico, deve ser possível mudar sua posição das atividades no tópico, levando em consideração que duas atividades não podem está na mesma posição em um tópico e nem existirem entre a ordenação como (0,2,3,4,15) ou números negativos.
## item 4
Deve ser possível alterar o tópico de uma atividade, perdendo sua posição no tópico antigo e ganhando uma posição no tópico para qual foi realocada, a nova posição deve ser determinada pelo membro que está alterando o tópico da atividade.
## item 5
Precisa-se aplicar a regra de ordenação nos tópicos em um projeto que deve seguir a regra contida no **item 3**.
## item 6
Tópicos não podem mudar de projeto apenas alterar seu index através do campo **index_on** dentro do mesmo projeto.
## item 7
Todas as entidades devem ter todos os campos gerenciáveis, possibilitando listagem, cadastro, visualização, edição e exclusão.
## item 8
 - Ao excluir um projeto não pode-se ter acesso aos demais dados do projeto como suas atividades, membros e tópicos.
 - Ao excluir um tópico as atividades pertencentes devem ser excluídas.
 - Ao excluir um membro este não deve poder visualizar os dados do projeto.
 - Ao ser excluir todos os membros do projeto deve-se apagar todos os dados do projeto
### O que iremos avaliar:
- Validação de requisições
- Logs da aplicação
- A organização do seu projeto e a forma que seu código foi escrito.
- Se a sua solução atende tudo que foi solicitado.
- Se preocupou com performance da aplicação.
- Manutenibilidade do código.
- Cobertura de código nos >= a 70%.
- Você entregou um readme com tudo que precisamos para executar.
### Itens que nos deixam com mais vontade de ter você no nosso time:
- Seu repositório contém algum tipo de script que cria o bando de dados e toda a "infra" necessária para a execução.
- Você foi além, e conseguimos testar a aplicação acessando uma versão que você deixou rodando em algum host público.
- Você foi mais além ainda, e conseguimos rodar localmente apenas baixando uma imagem docker ou dando um docker-compose up.
- Seu repositório tem algum tipo de automação compile o projeto e rode os testes.
- A sua API possui documentação (eu li swagger?).
- Anexar um arquivo json das rotas criadas importadas no insomnia.
### Envio
- Realizar o dump da base de dados e enviar em conjunto com os dados do projeto para um repositório publico no github com nome **Teste-Backend-InCicle-{seu-ultimo-sobrenome}** e envie o link para <recrutamento@incicle.com> seu nome completo no corpo do email.