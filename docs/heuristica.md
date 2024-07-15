## Heurística para identificação de classes
### Extração de substantivos

#### H1
 - Acesso
 - IP
 - MAC
 - Verificar acesso
 - Verificar certificado HTTPS
   
| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| Acesso | ip     | verificaCertificado | | |
|        | mac    | verificaAcesso      | | |

#### H2
 - Login
 - Usuário
 - Senha
 - Esqueci minha Senha
 - Troca de senha
 - Verificar troca de senha a cada 30 dias
 - 
| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| Login | usuario | login                | | |
|       | senha   | logout               | | |
|       |         | verificaLogin        | | |
|       |         | esqueciMinhaSenha    | | |
|       |         | verificaTrocaDeSenha | | |
|       |         | trocaDeSenha         | | |

### H3
 - Perfis de Usuário
 - Incluir, editar, excluir
 - Níveis de acesso
 - Nome do Perfil
 - Áreas
 - Areas principais e sub áreas

| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| Perfil | idPerfil  | incluir              | | |
|        | nome      | editar               | | |
|        | areas     | excluir              | | |
|        |           | niveisDeAcesso       | | |
|        |           | setAareasAcesso      | | |
|        |           | trocaDeSenha         | | |
| Area   | idArea    | setAreaPai           | | |
|        | nomeArea  | incluir              | | |
|        | idAreaPai | editar               | | |
|        | nivelArea | excluir              | | |


 #### H4
 - Usuários
 - Usuário
 - Senha
 - Email institucional
 - CPF
 - Data de Nascimento
 - Perfil
 - Email institucional
 - Inserir, editar Excluir
 - Resetar senha
 - Senha padrão
 - Critérios para senha

| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| Usuario | usuario    | incluir              |          | Usuarios |
|         | senha      | editar               |          | email    |
|         | cpf        | excluir              |          | |
|         | nascimento | resetSenha           |          | |
|         | idPerfil   | setSenhaPadrao       |          | |
|         | email      | validaCriteriosSenha |          | |

#### H5
 - Relatório de Entradas e Saídas
 - Filtros
 - Semana, Mês ou ano
 - Tipo de Material
 - Entradas/Saídas
 - Formatos
 - PDF, XLS
 - Permitir impressão
 - Exportar relatório
 - Busca relatório

| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| RelatorioEntradaSaida | dataInicio   | buscar   | | |
|                       | dataFim      | imprimir | | |
|                       | mes          | exportar | | |
|                       | ano          |          | | |
|                       | tipoMaterial |          | | |
|                       | entrada      |          | | |
|                       | saida        |          | | |
|                       | formato      |          | | |

#### H6
 - Relatório Balanço Anual
 - Produtos contabilidados
 - Balanco parcial
 - Balanco completo
 - Avisar usuários
 - Exportar balanço
 - Percentual contabilizado

| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| RelatorioBalancoAnual | tipoBalanco   | buscaContabilizados | | |
|                       | mensagem      | avisoUsuario        | | |
|                       |               | exportarBalanco     | | |

#### H7
 - Fechamento balanço anual
 - Nome
 - Data de fechamento balanço,
 - Status balanço
 - Parecer balanço
 - Inserir parecer final
 - Editar parecer final
 - Enviar alerta parecer

| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| BalancoAnual  | idBalanco      | inserirParecer | | |
|               | dataFechamento | editarParecer  | | |
|               | nome           | enviarAlerta   | | |
|               | status         |                | | |
|               | parecer        |                | | |
|               | percentual     |                | | |
|               | mensagem       |                | | |

#### H8
 - Personalizar interface do sistema
 - usuario 
 - Fonte
 - tamanho da fonte
 - cor
 - layout
 - Aumentar/diminuir fonte
 - Mudar fonte
 - Mudar cor
 - Selecionar layout predefinido (banco, preto, personalizado)


| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| PersonalizaInterface | idlayout          | mudarTamFonte  | | Layout |
|                      | usuario           | mudarFonte     | | |
|                      | fonte             | mudarCor       | | |
|                      | tamFonte          |                | | |
|                      | cor               |                | | |
|                      | layoutPredefinido |                | | |
| LayoutPreto          |                   |                | | |
| LayoutBranco         |                   |                | | |
| LayoutPersonalizado  |                   |                | | |
 
 #### H9
 - Inserir requisição de compra
 - Produto
 - Quantidade
 - Fornecedor
 - Data prevista entrega
 - Dia
 - Mês
 - Ano
 - Jstificativa
 - Exibir Mensagem de erro
 - Gerar arquivo PDF
 - Enviar email
 - Consultar histórico
 - Data requisição
 - Produto
 - Quantidade
 - Motivo
 - Data de entrega,
 - Status da Requisição
 - Observações
 - inserir requisição
 - editar requisicao
 - excluir requisicao
 - Gerar número da requisição

| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| Produto              | idProduto          | incluir            | dia | motivo |
|                      | quant              | editar             | mes |        |
|                      | idFornecedor       | excluir            | ano |        |
|                      | dataEntrega        |                    |     |        |
|                      | data               |                    |     |        |
| RequisicaoCompra     | justificativa      | incluir            |     |        |
|                      | statusRequisicao   | editar             |     |        |
|                      | nroRequisicao      | excluir            |     |        |
|                      | observacoes        | gerarNroRequisicao |     |        |
|                      | mensagem           | consultarHistorico |     |        |
|                      | data               | enviarEmail        |     |        |
|                      |                    | gerarPdf           |     |        |
|                      |                    | exibirErro         |     |        |
| Fornecedor           | idFornecedor       | incluir            |     |        |
|                      | nome               | editar             |     |        |
|                      |                    | excluir            |     |        |

#### H10
 - Inserir produtos
 - Editar produtos
 - Excluir produtos
 - Consultar produtos
 - Produto
 - Nome
 - Código
 - Descrição
 - Preço
 - Quantidade
 - Fornecedor
 - Validar campos
 - Código de barra
 - Fornecedor
 - Exibir mensagem de confirmação
 - Validar valores numericos

| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| Produto              | idProduto          | incluir                | | validarCampos |
|                      | quant              | editar                 | |               |
|                      | idFornecedor       | excluir                | |               |
|                      | dataEntrega        | consultar              | |               |
|                      | data               | validaValoresNumericos | |               |
|                      | preco              | mensagemConfirmacao    | |               |
|                      | codigoDeBarras     |                        | |               |

#### H11
 - Gerar relatórios de produtos
 - Relatorios
 - Produtos
 - Gerar relatório
 - Exportar relatório em PDF
 - Visualizar relatório em PDF
 - Armazenar relatório
 - Data
 - Hora

| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| Relatorios           | idRelatorio | exportarEmXLS          | | Produtos |
|                      | data        | exportarEmPDF          | | |
|                      | hora        | visualizarRelatorio    | | |
|                      |             | armazenarRelatorio     | | |
| RelatorioProdutos    |             |                        | | |

#### H12
 - Melhorias
 - Feedback
 - Enviar por email
 - Modo
 - Anonimo
 - Identificado
 - Numero protocolo
 - Busca

| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| SugestaoMelhorias    | idSugestaoMelhoria  | inserir                | | Identificacao |
|                      | modo                | editar                 | | Anonimo       |
|                      | protocolo           | excluir                | |               |
|                      | idUsuario           | buscar                 | |               |
|                      | feedback            | inserirFeedback        | |               |
|                      | sugestaoMelhoria    |                        | |               |

#### H13
 - Personalizar relatórios
 - Criar pastas
 - Selecionar dados
 - Tipos de relatórios (vendas, iventário e movimentação de estoque)

| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| Vendas              | |             | Personalizar relatórios | Criar pastas |
| Iventario           | |             |                         |              |
| MovimentacaoEstoque | |             |                         |              |

#### H14
 - Retornar dados
 - Uploads
 - Formatos CSF, Excel e JSON
 - Atualizar informações
 - Notificar usuário sobre uploads grandes
 - Notificações de atualização
 - Notificação de processamento
 - Atualizar relatórios

| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| RetornarDados  | idUsuario   | atualizarInformacoes | Uploads | Atualizar relatorios         |
|                | idRelatorio | notificarUsuario     |         | Notificacao de Processamento |
|                |             | notificarAtualizacao |         |                              |

#### H15
 - Alertas inteligentes
 - Problemas logísticos
 - Identificar problmeas logísticos
 - Falhas de estoque
 - Desvios na cadeia de suprimentos
 - Falha de fornecedor
 - Alertas por email
 - Analise de dados
 - Ajustar previsões de demanda

| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| Alertainteligente  | idUsuario   | problemasLogisticos     | Analise de dados             | Identificar Problemas Logisticos |
|                    |             | falhasDeEstoque         | Ajustar provisoes de demanda |                                  |
|                    |             | desvioCadeiaSuprimentos |                              |                                  |
|                    |             | falhaDeFornecedor       |                              |                                  |

#### H16
 - App mobile
 - Relatórios detalhados
 - Histórico de movimentação de estoque
 - Previsões de demanda
 - Status de reabastecimento
 - Personalizar relatório
 - Atualizar relatório
 - Data
 - Hora

| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| AppMobile          | idUsuario   | relatorioDetalhado     | | |
|                    | idRelatorio | historicoMovimentacao  | | |
|                    | data        | provisoesDeDemanda     | | |
|                    | hora        | personalizarRelatorio  | | |

#### H17
 - Verificar estoque
 - Vender
 - Clietne
 - Relatório de produtos em formato PDF
 - Ler QRCODE

| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| Venda            | idVenda    |                     | | |
|                  | idProduto  |                     | | |
|                  | qrCode     |                     | | |
|                  | quantidade |                     | | |
|                  | idCliente  |                     | | |
| VerificaEstoque  |            | consultarEstoque    | | |
|                  |            | inserirProduto      | | |

#### H18
 - Produtos à vencer
 - Alerta de produtos
 - Emitir relatório
 - Produtos vencidos ou com avarias


| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| ProdutosAVencer  | idProduto  | produtosAVencer           | | |
|                  |            | alertaProdutos            | | |
|                  |            | relatorioProdutos         | | |
|                  |            | produtosVencidosAvarias   | | |

#### H19
 - Atendimento
 - Chat
 - Vendedor
 - Emitir comprovante
 - Data
 - Hora
 - Compra
 - Garantida do produto
   

| classes candidatas | Atributos | Métodos | Info. Estanha | Redundância |
| --- | --- | --- | --- | --- |
| Venda            | idVenda       | inserir             | Compra | |
|                  | idProduto     | editar              |        | |
|                  | idCliente     | cancelar            |        | |
|                  | data          | emitirComprovante   |        | |
|                  | hora          | atualizarTotal      |        | |
|                  | valortotal    |                     |        | |
|                  | idVendedor    |                     |        | |
| ItemVenda        | idVenda       | inserirProduto      |        | |
|                  | idProduto     | removerProduto      |        | |
|                  | quantidade    |                     |        | | 
|                  | precoUnitario |                     |        | | 
|                  | garantia      |                     |        | | 


