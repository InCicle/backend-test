### Sobre a InCicle
A InCicle é uma empresa de tecnologia com foco em soluções para sistemas de gestão, recursos humanos e relacionamentos profissionais.
### Teste Backend
Esse teste consiste em conhecermos um pouco o seu conhecimento na área de desenvolvimento de **apis rest**.
Sendo assim, avaliaremos o seu domínio das linguagem Php ^8.x utilizando o framework Laravel ^10.x.
### Descrição da API
Desenvolver uma Api que atenda à modelagem disponibilizada abaixo(não necessário se limitar a ela), está api deve ser construida com a finalidade de gerenciar atividades de um projeto que podem ser visualizadas por membros desse projeto adicionados pelo administrador.

### DIAGRAMA

![Diagrama](https://github.com/InCicle/backend-test/blob/main/DER-testes.png?raw=true)

### **Requisitos**
## item 1
Essa api deve trabalhar com autorização para somente membros de um projeto possa gerenciar as atividades.
## item 2
Deve existir dois tipos de membros, membros comuns que tem permissão somente para gerenciar atividades e tópicos e os membros administradores que tem permissão de gerenciar todas as entidades com exceção da entidade person.
## item 3
Como apresentado no diagrama as atividades ficam agrupadas em tópicos, onde possuem um campo chamado **index_on** ordenado em ordem crescente (0,1,2,3,4...) que guarda a sua posição da atividade dentro do tópico, deve ser possível mudar sua posição das atividades no tópico, levando em consideração que duas atividades não podem está na mesma posição em um mesmo tópico, não existirem lacunas entre a ordenação como (0,2,3,4,15) e números negativos.
## item 4
Deve ser possível alterar o tópico de uma atividade, perdendo sua posição no tópico antigo e ganhando uma posição no tópico para qual foi realocada, a nova posição deve ser determinada pelo membro que está alterando o tópico da atividade.
## item 5
Precisa-se aplicar a regra de ordenação nos tópicos em um projeto que deve seguir a regra contida no **item 3**.
## item 7
Todas as entidades devem ter todos os campos gerenciáveis, possibilitando listagem, cadastro, visualização, edição e exclusão.
## item 8
 - Ao excluir um projeto não pode-se ter acesso aos demais dados do projeto como suas atividades, membros e tópicos.
 - Ao excluir um membro este não deve poder visualizar os dados do projeto.
## item 9
 - Dentre as rotas da aplicação construir uma rota que retorne as atividades em **andamento**(atividades sem data definida ou dentro do prazo), **atrasadas** e **concluídas** dado um membro do projeto, lembrando que o usuário deve ser membro da atividade para que esta entre no calculo.

### O que iremos avaliar:
- Validação das informações que serão gravadas
- Logs da aplicação
- A organização do seu projeto e a forma que seu código foi escrito.
- Se a sua solução atende tudo que foi solicitado.
- Você entregou um readme com tudo que precisamos para executar.
### Itens que nos deixam com mais vontade de ter você no nosso time:
- Se preocupou com performance da aplicação.
- Manutenibilidade do código.
- Cobertura de código nos >= a 70%.
- Anexar um arquivo json das rotas criadas importadas no insomnia.
### Envio
- Realizar o dump da base de dados e enviar em conjunto com os dados do projeto para um repositório publico no github com nome **Teste-Backend-InCicle-{seu-ultimo-sobrenome}** e envie o link para <recrutamento@incicle.com> seu nome completo no corpo do email.