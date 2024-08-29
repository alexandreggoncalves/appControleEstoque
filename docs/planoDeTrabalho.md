#  Sistema de Controle de Estoque - Meu Estoque Fácil - Plano de trabalho

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
| 1.1   | Planejamento do objeto, motivação, justificativa e oportunidade. Objetivo | Luciele I. Menezes| 02/06/2024|
| 1.2    |  Ajustes dos tópicos classes, equadrabilidade, tipo e equipe de projeto  | Luciele I. Menezes| 06/06/2024|

<p align="center"><b>Índice</b></p>

### 1. Introdução
  - 1.1 Objeto
    
     Este documento detalha a construção do sistema Meu Estoque Fácil, destacando as seções essenciais que servirão de alicerce para a definição dos requisitos e o desenvolvimento do sistema, tais como objetivo do sistema, visäo geral, requisitos e outros.   

  
  - 1.2 Motivação, Justificativa e Oportunidade
    
    O sistema de estoque atual, SESTOQUE, não mais atente as demandas do setor de forma eficaz neste estabelecimento comercial e pode gerar diversos problemas, como rupturas de estoque, 
perdas de produtos, descontrole da validade e dificuldade na tomada de decisões. Isso impacta diretamente na lucratividade do negócio,como na satisfação dos clientes e na capacidade de expansão. Implementar um sistema de estoque eficiente é importante para garantir o controle preciso dos produtos, reduzir custos, otimizar processos e impulsionar o crescimento do negócio. O investimento em um sistema de estoque adequado trata-se de uma decisão estratégica que trará benefícios a longo prazo, proporcionando organização,eficiência e eficácia para o gerenciamento do negócio.


  - 1.3 Caracterização do Projeto
    
    O novo sistema deverá ser desenvolvido em plataforma Web, em protocolo HTTPS e será concebido com a finalidade de controlar as áreas de planejamento, estocagem e distribuição de materiais. Todas as requisições serão em tempo real, possibilitando a integração entre os setores. O sistema ainda deverá ter:
    * Login baseado em usuário e senha;
    * Cadastro de usuários;
    * Cadastro perfis de uso;
    * Cadastro de fornecedores;
    * Cadastro de produtos;
    * Cadastro de categorias;
    * Controle de entrada de materiais;
    * Controle de saída de materiais;
    * Emissão de etiquetas de identificação;
    * Relatórios gerencias;
    * Controle de iventário/patrimônio;
    * Controle de WMS (Warehouse Management System)


 - 1.3.1 Integração com outros sistemas
   - Clientes: base de clientes da empresa;
   - Vendas: Sistema de Vendas local/online.
   - Compras: Sistema de Compras


  - 1.3.2 Classe

  | Classe        | Detalhamento                 |
| ----------------------- | ---------------------------------- |
| Sistema Web    |  Com acesso HTTPS, desenvolvido em PHP para controle de estoque com movimentação de entrada e saída de materiais.|              


     
    
  - 1.3.3 Enquadrabilidade
    
   | Enquadrabilidade        | Detalhamento                 |
| ----------------------- | ---------------------------------- |
| Sistema de uso comercial | Deve ser enquadrado sua base de desenvolvimento os 4 pilares de um sistema de estoque: (1) Previsão de demanda, (2) Tempo de Reposição, (3) Ponto de Pedido e (4) Contagem de Inventário |



  - 1.3.4 Tipo

  | Tipo       |                |   Detalhamento |
| -------------| ---------------|------------------ |
|Desenvolvimento | Software | Sistema WEB, em nuvem e com design responsivo a acesso via celulares, tablets, notebooks e computadores.|
       
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
      * relatórios gerenciais assertivos com clareza de informações.

### 3. Metodologia do Projeto

-  3.1 Estrutura do projeto

    - **Product Owner (PO)**
    - **Scrum Master (SM)**
    - **Gerente de Projeto**
    - **Equipe de Levantamento de Requisitos**
    - **Equipe de Desenvolvimento FRONTEND/BACKEND**
    - **Equipe de Implantação e Testes**
    - **Equipe de Suporte Técnico**

-  3.2 Equipe de Projeto: Papéis e Responsabilidades dos integrantes

| Papéis   |   Profissional             |  Responsabilidade |
| -------------| ---------------|------------------ |
| Product Owner (PO) |Prof. Dr. Andrey Rodrigues  | Responsável pelo desenvolvimento, traduz a voz do cliente em funcionalidades tangíveis. Defensor incansável, prioriza as necessidades, guiando a equipe à excelência do produto final.|
| Scrum Master (SM) |Alexandre Gomes Gonçalves  |  Assume o papel crucial de líder e facilitador, guiando a equipe rumo ao sucesso do projeto. Ele garante a aplicação dos princípios e valores do Scrum, promovendo a colaboração, a auto-organização e a entrega de valor para o cliente.|
|Time Squad| Ester Castro, Erikson, Luciele I. Menezes, |Atuam na projeção, desenvolvimento, testes e na implementação das funcionalidades do sistema.|
| Designer UX | Alexandre Gomes Gonçalves  |  Deverá ter a função de criar elementos gráficos, como ícones, botões, layouts e tipografia, que tornam a interface esteticamente agradável e atraente.|
| Suporte Técnico | Luciele I. Menezes  |  Atua como a linha de frente na resolução de problemas e dúvidas relacionadas a produtos, serviços ou sistemas. Suporte na construção do  Plano de Trabalho e no levantamento dos requisitos e criação de user story|
| Desenvolvedores de FRONTEND/BACKEND | Ester Castro de Oliveira |  Encarregada pela criação e implementação da interface de um site ou aplicativo, com foco na experiência do usuário. É responsável também por planejar, programar, testar e manter a estrutura de códigos que faz a interface entre um site, o servidor e o banco de dados. | 
| Implantação e Testes | Alexandre Gomes Gonçalves | Responsável por identificar erros, falhas ou comportamentos inesperados no software durante os testes. |
| Suporte Técnico | Ester Castro | Responsável por diagnosticar e resolver problemas técnicos e oferecer suporte remoto ou presencial aos usuários, além de documentar e reportar incidentes e soluções. |

- 3.3 Fases, Atividades e Cronograma

    Fase I: Especificação – Maio/Junho:
    Fase II: Inspeção - Julho/Agosto 
    Fase III: Projeto e Arquitetura - Setembro/Outubro
    Fase IV: Prototipagem e Refinamento - Novembro
    Fase V: Encerramento - Dezembro

  - 3.4 Entregas de cada fase

    | Fase | Mês | Entregável |
    | --- | --- | --- |
    | I - Especificação | Junho | - Plano de Trabalho<br> - Definição de Personas<br> - Criação de User Story<br> - Especificação dos requisitos do Sistema |
    | II - Inspeção | | |
    | III - Prototipagem e Refinamento | | |
    | IV - Encerramento | | |

- 3.5 Controle de Mudanças

O monitoramento e controle do escopo do projeto serão realizados a partir das seguintes diretrizes:

  - Requisitos do projeto devem ser compreendidos por todos os membros da equipe.
  - Todas as questões técnicas, de entregas e do cronograma que a equipe do projeto possui devem ser respondidas.
  - Todas as entregas devem ser acordadas pela equipe do projeto e entidades parceiras.
  - Todas as informações devem estar atualizadas no escopo e não-escopo.
  - Nenhum trabalho fora do escopo do projeto deve ser feito.
  - Solicitações de mudança no escopo do projeto devem ser efetivamentecomunicadas e compreendidas.
