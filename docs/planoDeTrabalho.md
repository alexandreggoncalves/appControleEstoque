# APP - Controlde de Estoque - Plano de trabalho

| Nome do Projeto:        | Meu Estoque Fácil                  |
| ----------------------- | ---------------------------------- |
| Versão:                 | **1.0**                            |
| Status:                 | **Planejamento e Pesquisa**        |
| Executor Principal:     | discente Alexandre Gomes Gonçalves |
| Coordenador do Projeto: | Prof. Dr. Andrey Rodrigues         |

# Histórico de Versões
| Versão | Descrição | Autor | Data |
| :---: | --- | --- | :---: |
| 1.0   | Planejamento e pesquisa | Alexandre G. Gonçalves | 28/05/2024 |
| 1.1   | Planejamento do objeto, motivação, justificativa e oportunidade. Objetivo | Luciele I. Menezes| 02/05/2024|
|       |                         |                        |            |
|       |                         |                        |            |
|       |                         |                        |            |

<p align="center"><b>Índice</b></p>

### 1. Introdução
  - 1.1 Objeto
    
     Este documento detalha a construção do sistema Meu Estoque Fácil, destacando as seções essenciais que servirão de alicerce para a definição dos requisitos e o desenvolvimento do sistema, tais como objetivo do sistema, visäo geral, requesitos e outros.   

  
  - 1.2 Motivação, Justificativa e Oportunidade
    
    O sistema de estoque atual, SESTOQUE, não mais atente as demandas do setor de forma eficaz neste estabelecimento comercial e pode gerar diversos problemas, como rupturas de estoque, 
perdas de produtos, descontrole da validade e dificuldade na tomada de decisões. Isso impacta diretamente na lucratividade do negócio,como na satisfação dos clientes e na capacidade de expansão. Implementar um sistema de estoque eficiente é importante para garantir o controle preciso dos produtos, reduzir custos, otimizar processos e impulsionar o crescimento do negócio. O investimento em um sistema de estoque adequado trata-se de uma decisão estratégica que trará benefícios a longo prazo, proporcionando organização,eficiência e eficácia para o gerenciamento do negócio.


  - 1.3 Caracterização do Projeto
    
    O novo sistema deverá deverá ser desenvolvido em plataforma Web, em protocolo HTTPS e será concebido com a finalidade de controlar as áreas de planejamento, estocagem e distribuição de materiais. Todas as requisições serão em tempo real, possibilitando a integração entre os setores. O sistema ainda deverá ter:
    * login baseado em usuário e senha;
    * cadastro de usuários;
    * cadastro perfis de uso;
    * cadastro de fornecedores;
    * cadastro de produtos;
    * cadastro de categorias;
    * controle de entrada de materiais;
    * controle de saída de materiais;s;
    * emissão de etiquetas de identificação;
    * relatórios gerencias;
    * controle de iventário/patrimônio;
    * controle de WMS (Warehouse Management System)


 - 1.3.1 Integração com outros sistemas
   - Clientes: base de clientes da empresa;
   - Vendas: Sistema de Vendas local/online.
   - Compras: Sistema de Compras


  - 1.3.2 Classe

  | Classe        | Detalhamento                 |
| ----------------------- | ---------------------------------- |
| Sistema Web             |  com acesso HTTPS, desenvolvido em PHP para controle de estoque com movimentação de entrada e saída de materiais.                        |
|                 |       |


     
    
  - 1.3.3
    
    | Enquadrabilidade        | Detalhamento                 |
| ----------------------- | ---------------------------------- |
| Sistema de uso comercial | Contempla os atuais requisitos logísticos de controle de armazenamento e movimentação de materiais.                        |
|                 |       |


  - 1.3.4 Tipo
      Desenvolvimento de sistema WEB, em nuvem e com design responsivo a acesso via celulares, tablets, notebooks e computadores.

    
     
### 2. Informações Gerais
  - 2.1 Objetivo

      Desenvolver um sistema de estoque eficiente para otimizar o gerenciamento dos produtos, reduzir custos, aumentar a lucratividade e impulsionar o crescimento do negócio.
    
  - 2.2 Escopo Geral

      O sistema deverar permitir a integração entre o processo produtivo e o controle de estoque, garantido o fornecimento contínuo de materiais, bem como auxiliar o setor de compras e vendas.
    
  - 2.2.1 Escopo Eespecífico
    - Cadastro de Produtos;
    - Controle de movimentação, entrada/saída;
    - Relatórios gerenciais e balanços;
    - Controle de armazenamento de materiais.

  - 2.2.2 Escopo Negativo
      - Não há API para consulta de terceiros;
      - Acessível somente ao setor de estoque/almoxarifado;
      - Não realiza compras e nem vendas, somente movimentação de entrada e saída de materiais.

  - 2.3 Ambiente de Desenvolvimento

    **Ferramentas e Tecnologias**
    | Tipo             | Especificações                        |
    | ---              | ---                                   |
    | PHP Storm | IDE para desenvolvimento de aplicações em PHP |
    | MySQL Server | Servidor de Banco de Dados relacional |
    | MySQL Workbanch | Ferramenta para design do Banco de Dados |
    | Adobe Photoshop | Ferramenta gráfica para criação do design |
    | Frontend e Backend | Java, Node.js, HTML5, Bootstrap |
    | Scrum | Metologia de gerenciamento de Projetos |
    | Git | Sistema de controle de Versões | 
    | Hospedagem | HostGator |

  - 2.4 Características Inovadoras do Projeto
    * aplicação WEB com tecnologias atuais;
    * acessibilidade a qualquer dispositivo que acesse plataformas Web;
    * WMS (Warehouse Management System), para gerenciar o armazenamento de localização dos materiais;
    * etiquetamento de mercadorias com QR code;
    * dados disponíveis em tempo real.
    
     
  - 2.5 Resultados Esperados
      * espera-se um maior controle e automatização do estoque;
      * simplificação de processos e confiabilidade nos dados;
      * relatórios gerenciais acertivos com clareza de informações.

### 3. Metodologia do Projeto

-  3.1 Estrutura do projeto
    - **Gerente de Projeto**
    - **Equipe de Levantamento de Requisitos**
    - **Equipe de Desenvolvimento FRONTEND/BACKEND**
    - **Equipe de Implantação e Testes**
    - **Equipe de Suporte Técnico**

-  3.2 Equipe de Projeto: Papéis e Responsabilidades dos integrantes

   * **Alexandre Gomes Gonçalves**, tem a responsabilidade de gerenciar o projeto e o repositório GIT, verificar o andamento dos processos, desenvolvimento do perfil das "personas" que utilizarão o sistema, auxiliará no levantamento de requisitos.
