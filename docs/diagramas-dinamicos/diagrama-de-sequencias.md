# Diagrama de Sequências - Meu Estoque Fácil

## Gerente
O Gerente inicia o processo fazendo login no sistema, fornecendo seu nome de usuário e senha. O sistema valida essas credenciais consultando o banco de dados. Se as credenciais forem válidas, o Gerente pode navegar para a página de perfis. Na página de perfis, o Gerente insere um novo perfil, especificando o nome do perfil e as áreas de acesso associadas a ele. O sistema valida os dados do perfil novamente consultando o banco de dados. Se os dados do perfil forem inválidos, o sistema retorna uma mensagem de erro informando que os dados são inválidos. Se os dados forem válidos, o sistema salva o novo perfil no banco de dados e retorna uma mensagem de sucesso informando que o perfil foi inserido com sucesso.

![alt Gerente](https://github.com/alexandreggoncalves/appControleEstoque/blob/main/docs/diagramas-dinamicos/diagrama_sequencia_gerente.jpeg)

## Operador de Reposição
O Operador de Reposição começa fazendo login no sistema com seu nome de usuário e senha. O sistema valida essas credenciais consultando o banco de dados. Com as credenciais validadas, o Operador pode navegar para a página de produtos. Na página de produtos, o Operador insere um novo produto, fornecendo o nome, código, descrição, preço, quantidade e fornecedor do produto. O sistema valida os dados do produto consultando o banco de dados. Se os dados do produto forem inválidos, o sistema retorna uma mensagem de erro indicando que os dados são inválidos. Se os dados forem válidos, o sistema salva o novo produto no banco de dados e retorna uma mensagem de sucesso indicando que o produto foi inserido com sucesso.

![alt Operador de Reposição](https://github.com/alexandreggoncalves/appControleEstoque/blob/main/docs/diagramas-dinamicos/diagrama_sequencia_operador_de_reposicao.jpeg)


## Operador de Movimentação
O Operador de Movimentação inicia o processo fazendo login no sistema com seu nome de usuário e senha. O sistema valida essas credenciais consultando o banco de dados. Uma vez autenticado, o Operador pode navegar para a página de entradas. Na página de entradas, o Operador registra uma nova entrada, especificando o produto, a quantidade, a localização e a data da entrada. O sistema valida os dados da entrada consultando o banco de dados. Se os dados forem inválidos, o sistema retorna uma mensagem de erro informando que os dados são inválidos. Se os dados forem válidos, o sistema salva a nova entrada no banco de dados e retorna uma mensagem de sucesso informando que a entrada foi registrada com sucesso.

![alt Operador de Movimentação](https://github.com/alexandreggoncalves/appControleEstoque/blob/main/docs/diagramas-dinamicos/diagrama_sequencia_operador_de_movimentacao.jpeg)


## Operador de Fechamento
O Operador de Fechamento faz login no sistema com nome de usuário e senha. O sistema valida as credenciais junto ao banco de dados e, se válidas, permite o acesso. O operador então navega para a seção de relatórios e emite um relatório de fechamento especificando tipo, período e filtro de material. O sistema obtém os dados do fechamento do banco de dados e exibe o relatório. O operador pode optar por exportar o relatório como PDF ou XLS, com o sistema realizando a exportação e confirmando o sucesso.

![alt Operador de Fechamento](https://github.com/alexandreggoncalves/appControleEstoque/blob/main/docs/diagramas-dinamicos/diagrama_sequencia_operador_de_fechamento.jpeg)


## Operador de Vendas
O Operador de Vendas realiza o login no sistema com nome de usuário e senha. O sistema valida as credenciais junto ao banco de dados e, se válidas, permite o acesso. O operador navega para a seção de consulta de estoque e consulta um produto fornecendo nome e código. O sistema busca as informações no banco de dados e exibe os resultados ao operador.

![alt Operador de Vendas](https://github.com/alexandreggoncalves/appControleEstoque/blob/main/docs/diagramas-dinamicos/diagrama_sequencia_operador_de_vendas.jpeg)

