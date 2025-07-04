# Requisitos do Sistema Meu Estoque Fácil

## Perfis de usuário:
  * Gerente:
      * Inserir, editar e excluir usuários
         * Esta funcionalidade tem como objetivo permitir a inclusão, alteração ou exclusão de usuários e suas credenciais no sistema.
         
      * Emitir relatórios gerenciais
         * Esta funcionalidade permite aos gerentes e supervisores emitir relatórios de entrada e saída de materiais para controle do estoque.
           
      * Supervisionar a movimentação de entrada e saída de materiais
         * Esta funcionalidade permite ao operador do estoque controlar os materias, sejam eles de entrada no estoque ou saída.
           
      * Validar o fechamento anual
         * A validação do fechamento do estoque, ocorre anualmente e faz-se necessário para iniciar um novo ano de trabalho.

  * Operador de Reposição: 
      * Inserir, editar ou excluir produtos do sistema
         * Aqui o operador de reposição pode inserir novos produtos, editar os existentes e excluir produtos caso haja alguma divergência.
         
      * Inserir requisição de compra ao setor de compras
         * A requisição de compra existe para que o operador de reposição possa solicitar novos produtos ao setor de compras.
           
      * Gerar relatórios de estoque
         * Os relatórios gerados aqui, vão auxiliar o operador de reposição a controlar o estoque e os materiais.
     

  * Operador de Movimentação:
      * Realizar movimentação de entrada de materiais no estoque
         * Funcionalidade para que o operador de movimentação possa dar entrada de produtos no sistema.
           
      * Realizar movimentação de saída de materiais no estoque
         * Funcionalidade para que o operador de movimentação possa dar saída de produtos no sistema.
           
  * Operador de Fechamento:
      * Verificar divergências no estoque relativo a quantidades e disponibilidade dos produtos
         * Esta funcionalidade permite ao operador de fechamento apontar e solucionar as divergências, caso ocorram, no estoque.
           
      * Verificar fechamento semanal do estoque
         * A verificação de fechamento server para semanalmente apontar problemas de estoque e poder solucionar elas mais rapidadmente.
           
      * Emitir relatórios de fechamento
         * Os relatórios de fechamento servem para arquivamento físico de fechamento do estoque.
           
      * Realizar o fechamento anual do estoque
         * O operador de fechamento que verifica, soluciona e autoriza o fechamento anual do balanço de estoque.

  * Operador de Vendas:
      * Consultar o sistema de estoque para realizar a venda de produtos
      * Solicitar produtos para o balcão de vendas
      * Solicitar produtos para o balcão físico da loja
   
  | **Risco**                                                                | **Impacto** | **Probabilidade** | **Plano de Ação**                                                                                 |
| ------------------------------------------------------------------------ | ----------- | ----------------- | ------------------------------------------------------------------------------------------------- |
| Exclusão acidental de usuários ou perda de credenciais                   | Alto        | Média             | Implementar confirmação em duas etapas para exclusão e backup automático das credenciais.         |
| Geração de relatórios com dados inconsistentes ou desatualizados         | Alto        | Média             | Garantir sincronização em tempo real com o banco de dados e aplicar validações antes da emissão.  |
| Falta de permissão adequada para operador supervisionar movimentações    | Médio       | Alta              | Implementar controle de permissões por função e registrar logs de acesso e operação.              |
| Ambiguidade sobre quem realiza a supervisão de movimentação              | Médio       | Média             | Especificar claramente no sistema quem tem papel de supervisão (Gerente ou Operador).             |
| Validação incorreta do fechamento anual por falta de critérios definidos | Alto        | Média             | Definir critérios claros de validação e implementar checklist obrigatório no sistema.             |
| Esquecimento do fechamento anual e impacto na continuidade do sistema    | Alto        | Baixa             | Programar alertas automáticos e bloqueios parciais no sistema após a data limite.                 |
| Conflitos entre permissões de gerente e supervisor                       | Médio       | Média             | Documentar claramente a hierarquia de permissões e aplicar testes de usabilidade com os usuários. |
| Falta de rastreabilidade nas alterações de usuários e movimentações      | Alto        | Alta              | Implementar auditoria detalhada (logs) para todas as ações críticas no sistema.                   |



**ID:** RF-01  
**Título:** Inserir novo usuário  
**Descrição:**  
O sistema deve permitir que um gerente insira novos usuários por meio de um formulário com campos obrigatórios.

**Critérios de Aceitação:**
- O formulário deve conter os campos: nome, e-mail, função, senha.
- Não deve permitir duplicidade de e-mail.
- O sistema deve exibir mensagem de sucesso após o cadastro.

**Requisitos Relacionados:** [ex: RF-02 – Editar usuário]

**Prioridade:** Alta  
**Volatilidade:** Baixa  
**Criticidade:** Alta

**Dependências:** Requer autenticação e permissões de gerente.


BANCO DE DADOS

| **Categoria**         | **Especificação**                                                                              |
| --------------------- | ---------------------------------------------------------------------------------------------- |
| **Desempenho**        | O banco de dados deve responder a consultas simples em no máximo 2 segundos.                   |
| **Confiabilidade**    | Deve manter a integridade dos dados mesmo em caso de falha do sistema ou queda de energia.     |
| **Segurança**         | Os dados sensíveis (ex.: senhas) devem ser armazenados usando criptografia hash (ex.: bcrypt). |
|                       | Deve haver controle de acesso baseado em permissões e logs de auditoria.                       |
| **Escalabilidade**    | O banco deve permitir crescimento do volume de dados sem perda significativa de desempenho.    |
| **Manutenibilidade**  | Deve permitir backup e restauração sem interrupções no serviço, com ferramentas automatizadas. |
| **Integridade**       | Chaves estrangeiras devem ser usadas para garantir relacionamentos corretos entre tabelas.     |
| **Disponibilidade**   | O banco deve estar disponível no mínimo 99% do tempo durante o horário comercial.              |
| **Portabilidade**     | O banco deve ser compatível com sistemas SQL como PostgreSQL e MySQL.                          |
| **Auditoria**         | Todas as alterações em dados críticos (usuários, movimentações) devem ser registradas em log.  |
| **Retenção de Dados** | Dados de movimentações devem ser mantidos por no mínimo 5 anos antes de possível arquivamento. |
| **Consistência**      | Transações devem seguir o modelo ACID (Atomicidade, Consistência, Isolamento e Durabilidade).  |
