### Sobre a InCicle

A InCicle é uma empresa de tecnologia com foco em soluções para sistemas de gestão, recursos humanos e relacionamentos profissionais.

### Teste Backend

Esse teste consiste em conhecermos um pouco o seu conhecimento na área de desenvolvimento de **apis rest**.
Sendo assim, avaliaremos o seu domínio das linguagem Php utilizando o framework Laravel.

## Tarefa 1

- Precisamos de um sistema para vendas.

### Descrição da tarefa 1

- Queremos controlar as vendas do dia. Pense em uma tela onde eu informo a data da venda, o cliente que comprou e a forma de pagamento (Dinheiro ou Cartão). Caso o pagamento seja do tipo Cartão é enviado para o gateway de pagamento, que aceita no máximo 10 pagamentos por minuto, sendo assim devemos realizar o controle de requisições para evitar perca de pedidos. Daí eu indico quais os produtos que o cliente comprou e a quantidade de cada itens por produto. O sistema me mostra o valor total da venda. Quando salvar a ordem de compra, liberar o download de uma cópia do pedido em PDF com o nome do cliente, a data da compra, a lista de pedidos comprados e valor total. Preciso ter um cadastro de produtos para não precisar digitar o nome do produto todas as vezes. Seria bom se pudesse ter um controle de usuários, para evitar que pessoas não autorizadas tenham acesso. E também uma listagem onde seleciono o cliente e são listados os pedidos dele.

### Informações Complementares referentes a tarefa 1

- A api que você vai enviar os pagamentos é ficticia e a sua url é um:
  
  ````
       POST https://pagamentos-test/send
  ````

- As informações que vai passar para o body da requisição é:

  ````
        {
            "card":"Número do cartão do comprador"
            "document":"número cpf ou cnpj do usuário",
            "type":"Typo de usuário cnpj/cpf",
            "value":"valor da compra",
            "buy_date":"data da compra",
        }
  ````

## Tarefa 2

- Criar uma base de dados usando as seeds do laravel e consultando a api https://pokeapi.co/ para cadastrar mil itens e trazer todos os dados no banco.
Após a inserção ser realizada, Criar uma rota que retorne esses dados e os guarde em um array, sua tarefa é, construir uma função que receba como parametro
o nome de um pokemon guardado dentro desse array e busque o mesmo dentro do array.

### Informações Complementares referentes a tarefa 2

- Não queremos consultas diretas no banco pelo nome dos pokemons.

### Envio

- Realizar o dump da base de dados e enviar em conjunto com os dados do projeto para um repositório publico no github com nome **Teste Backend InCicle** e envie o link para <recrutamento@incicle.com> seu nome completo no corpo do email.